# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

GreenSeal.dev is a Jekyll static site for a sustainability consulting company (GreenSeal Lda., Portugal). It promotes Green Software Practices (GSP) certification and consulting services. Hosted on GitHub Pages.

## Build Commands

```bash
bundle install            # Install Ruby dependencies
bundle exec jekyll serve  # Build and serve locally (http://localhost:4000)
bundle exec jekyll build  # Production build (output in _site/)
```

No test framework is configured.

## Architecture

**Stack:** Jekyll + Bootstrap 5.3.2 + SCSS, hosted on GitHub Pages via the `github-pages` gem.

### Layout Hierarchy

`base.html` (HTML shell, analytics, SEO meta) → `default.html` (header/footer/nav) → page-specific layouts (`home.html`, `service.html`, `blog.html`, `gsp.html`, `certified-company.html`, `team.html`, etc.)

### Collections (defined in `_config.yml`)

- **`_services/`** — Service offerings. Sorted by `weight` frontmatter. Output to `/services/`.
- **`_team/`** — Team members. Files prefixed with `_` are drafts/templates.
- **`_certified/`** — GSP-certified organizations. Permalink: `/gsp/certified/:name/`.
- **`/blog/`** — Blog posts. Date-prefixed filenames (`YYYY-MM-DD-slug.md`), layout `blog`.

### Data-Driven Content (`_data/`)

- `menus.yml` — Main and footer navigation menus (items have `weight` for ordering).
- `certification_levels.yml` — GSP certification tier definitions.
- `contact.yml` — Contact details used in templates.
- `social.json` — Social media links.
- `seo.yml` — SEO metadata.

### Styles (`_sass/` + `assets/css/style.scss`)

`style.scss` is the entry point — defines color variables, imports a selective subset of Bootstrap 5 (many components are commented out), then custom component and page SCSS files.

**Brand colors:** Primary `#427F69`, Primary Dark `#2C4436`, Secondary `#A3BDB3`.
**Fonts:** Helvetica/Arial (body), Playfair Display via Google Fonts (headings).

### JavaScript

Minimal — only `assets/js/scripts.js` handling mobile hamburger menu toggle. No build tooling or bundler.

## Content Conventions

### Adding a Service

Create a `.md` file in `_services/` with frontmatter: `title`, `weight` (sort order), `summary`, `date`. Layout defaults to `service` via `_config.yml`.

### Adding a Blog Post

Create `/blog/YYYY-MM-DD-slug.md` with frontmatter: `title`, `layout: blog`, `date`, `author`, `image`.

### Adding a Certified Organization

Create a `.md` file in `_certified/` with relevant frontmatter. Layout defaults to `certified-company`. Permalink pattern: `/gsp/certified/:name/`.

### Navigation

Edit `_data/menus.yml`. Items need `name`, `url`, and `weight` fields.

## Agent Team

Three specialized subagents live in `.claude/agents/` (which is excluded from the Jekyll build, along with `.claude/` generally, since dot-directories are excluded by Jekyll's default behavior and nothing in `_config.yml` overrides that). Route content and site work to them by role rather than doing it directly in the main thread.

### Agents

- **content-writer** — audience-facing prose: blog posts, LinkedIn copy, Services/GSP/About/Team/Contact page copy, outreach emails. Owns narrative, hooks, structure, and tone.
- **green-software-expert** — technical accuracy on anything involving green AI, sustainable software engineering, software quality, energy measurement, or standards (ISO/IEC TS 20125-1, RGESN, Blue Angel, GHG Protocol, SCI), or GSP itself. Required review gate before publishing anything with a technical or factual claim.
- **web-jekyll-marketing** — Jekyll implementation (layouts, front matter, includes, collections, navigation, build config), on-site SEO, and distribution mechanics (LinkedIn format, meta tags, OG images, forms) for any page on the site.

### Typical workflows

- **New blog post**: content-writer drafts → green-software-expert reviews technical claims → web-jekyll-marketing handles front matter/publishing and prepares the LinkedIn distribution format. Follow this order; don't skip the technical review step even for posts that feel low-risk.
- **Editing a standing page** (Services, GSP, About): check what the page currently says first. content-writer edits copy, green-software-expert confirms nothing drifts from how GSP or standards are defined elsewhere on the site, web-jekyll-marketing implements if the change touches layout, not just text.
- **Site changes with no content component** (performance, navigation, forms, redesign): web-jekyll-marketing alone, no need to route through the other two.

### House rules that apply across all agents

- No em dashes or en dashes in any copy. Use commas or full stops.
- Before creating new content, check what already exists (blog index, live page copy) so agents don't duplicate an angle or contradict a prior claim.
- Keep the site itself lean and fast. A sustainability consultancy with a bloated website undercuts its own message.

### Active content plan

The current blog pipeline is tracked in [`.claude/docs/blog-plan-2026-08.md`](.claude/docs/blog-plan-2026-08.md) (August–September 2026 series). Check it before starting new blog work to avoid duplicating a scheduled topic, and update its Status column as posts move through the pipeline.

## Key Details

- Files prefixed with `_` in collections (e.g., `_consulting.md`, `_sage-kirk.md`) are drafts/templates and not output by Jekyll.
- The GSP section (`/gsp/`) has its own sub-navigation via `_includes/gsp-nav.html`.
- Cookie consent is opt-in (analytics denied by default). See `_includes/cookie-banner.html` and `_layouts/base.html`.
- Plugins: `jekyll-environment-variables`, `jekyll-sitemap`.
