---
layout: blog
title: "How AI quietly rewrote Big Tech's climate promises"
date: 2026-10-12
author: Luís Cruz
tags: [green software, AI, sustainability, carbon accounting, Scope 2, GHG Protocol, climate claims]
description: "Goals became moonshots. Baselines became year-over-year. '100% renewable' became a yearly total. How Big Tech rewrote its climate promises for AI."
image: /images/blog/big-tech-climate-claims-ai.jpg
---

> In 2020, Microsoft promised to be carbon negative by 2030 and Google called 24/7 carbon-free energy "our biggest sustainability moonshot yet". Six years and one AI boom later, the companies' own data puts all four of the biggest cloud and AI providers roughly 60 to 80% above where they stood around the time they made those promises. The pledges were quietly reworked to fit. Goals became moonshots, baselines became year-over-year, "100% renewable" came to mean a yearly total rather than the power actually running the servers, and carbon-neutral claims were discontinued. Here is the scorecard, how the goalposts moved, and what to ask your AI vendors.

<figure class="figure mb-4 d-block">
  <img src="/images/blog/big-tech-climate-claims-ai.jpg" alt="How AI quietly rewrote Big Tech's climate promises" class="figure-img img-fluid rounded mb-1" />
  <figcaption class="figure-caption" style="font-size: 0.75rem;">Photo by Albert Stoynov</figcaption>
</figure>

In January 2020, Brad Smith wrote: "By 2030 Microsoft will be carbon negative."[^ms2020] Eight months later, Sundar Pichai announced that "by 2030 Google is aiming to run our business on carbon-free energy everywhere, at all times", and called it "our biggest sustainability moonshot yet".[^g2020] Amazon had already co-founded The Climate Pledge, net zero by 2040.[^amz2019] Facebook, now Meta, set "a goal to reach net zero emissions for our value chain in 2030".[^meta2021]

Then came the AI build-out. By May 2024, Smith was telling Bloomberg Green: "So in many ways the moon is five times as far away as it was in 2020."[^smith] In June 2026, Google's sustainability blog conceded that "reaching our climate moonshots is getting harder".[^gblog2026]

The headline targets are, technically, still on the page. Almost everything around them has been rewritten: the words, the metrics and the accounting. Start with the numbers.

## The scorecard

Each company's latest own-reported total, compared with the starting year its goal is measured against. For Microsoft, Google and Amazon that is the baseline year of their targets. Meta's net-zero pledge names no base year, so we use 2020, the year of the pledge.

| Company | Pledge | Latest total | vs baseline |
|---|---|---|---|
| Microsoft | Carbon negative by 2030 | 20.3 Mt (2025*) | +58% vs 2020* |
| Google | Net zero by 2030 | 14.5 Mt (2025) | +81% vs 2019 |
| Amazon | Net zero by 2040 | 80.9 Mt (2025) | +58% vs 2019 |
| Meta | Net zero value chain in 2030 | 8.2 Mt (2024) | +60% vs 2020 (+41% vs 2021) |
{: .table .table-sm}

Mt is million tonnes of CO2e across all emission scopes. Some percentages are our own calculation from the companies' reports, and several companies changed their methods along the way. *Microsoft reports by financial year, July to June.

<details class="notes" markdown="1">
<summary>How we calculated these numbers</summary>

- **Scopes.** Totals cover Scope 1 (direct emissions), Scope 2 (purchased electricity) and Scope 3 (the rest of the value chain).
- **Sources.** Microsoft, Amazon and Meta percentages are our calculation from the companies' own data tables. Google's +81% is its own figure.[^msfs][^gr2026][^amz2025][^meta2025] The comparisons are not perfectly like-for-like, and the companies' own methodology changes are part of the story.
- **Microsoft.** Microsoft reports by financial year, so 2025 means July 2024 to June 2025 and 2020 means July 2019 to June 2020. The figure uses its "management's criteria" series (+62% on its GHG Protocol-aligned series).[^kjmoon] Earlier years have been restated, so its previously published 29.1% and 23.4% increases[^ms2024][^ms2025] do not sit on the same line.
- **Google.** The figure uses an "ambition-based" metric Google introduced in 2025. It leaves out about 4.4 Mt that its GHG Protocol-aligned total (18.8 Mt, +82% vs 2019 by our calculation) includes.[^kjgoogle]
- **Amazon.** Amazon changed its carbon methodology from 2022 onward.
- **Meta.** Meta's latest published report is the 2025 one, covering calendar 2024. Its figure is before carbon removals. The +41% is against 2021, the base year of its science-based target. Its 2026 report was not out at the time of writing.

</details>

Google also set itself a second, harder target: 24/7 carbon-free energy, matched hour by hour on the same grid. In 2025 it reached about 65%, against 66% the year before.[^gr2026] Flat, four years out from a target of roughly 100%.

All four name data centres or AI as a driver. Microsoft attributes its 25% year-over-year rise "primarily" to "the expansion of our datacenter infrastructure" and to pausing its use of unbundled renewable certificates (more on that below).[^ms2026] Google says "our climate impact has been growing alongside the unprecedented growth of AI".[^gr2026] Amazon's chief sustainability officer writes that AI demand "may slow us down".[^amz2025] Meta says its value chain emissions "continue to fluctuate as our business expands and recently constructed data centers come online",[^meta2025] which is a gentle verb for a 60% rise.

So the numbers went the wrong way. Here is how the pledges were reworked to live with them.

## How the goalposts moved

### Goals became moonshots

"Moonshot" was in Google's 2020 announcement, so the word itself is not new. Its weight is. By our count of the report text, "net-zero goal" appears five times in Google's 2024 environmental report and not once in 2025 or 2026. Over the same three reports, "moonshot" goes from about four mentions to about fifteen, then about twenty. Treat the counts as indicative, but the direction is clear.

In mid-2025 Google also moved most net-zero references off the front of its sustainability site, with the pledge relocated to an appendix entry, according to Canada's National Observer, whose reporting on Google's shift toward moonshot language is what prompted our count.[^nco] Played down, not withdrawn: the 2026 report still states "We aim to reach net-zero emissions across all of our operations and value chain by 2030."[^gr2026] But a moonshot is something you are allowed to miss. A goal is not.

The rewording followed an earlier retreat. In its 2024 report, Google disclosed that "starting in 2023, we're no longer maintaining operational carbon neutrality". It had met that claim every year from 2007 to 2022 on the back of renewable matching and avoidance credits.[^gr2024]

### Baselines became year-over-year

Microsoft's 2024 report said emissions were "up 29.1% from the 2020 baseline".[^ms2024] Its 2025 report said "increased by 23.4% compared to our 2020 baseline".[^ms2025] Its 2026 report states the 25% year-over-year rise and does not state the cumulative change against 2020 in its text.[^ms2026] You have to work that out from the data fact sheet.

Amazon does something similar. It leads with carbon intensity, emissions per dollar of sales, which fell 38% from 2019 by our calculation. Over the same period the absolute total rose 58%.[^amz2025]

Microsoft's 2026 foreword is careful: "the context has evolved, and so must our approach", followed by "It does not mean we are lowering our ambition."[^ms2026] The carbon-negative target is still listed. We take that at its word, and note that the sentence was needed.

### "100% renewable" became a yearly bookkeeping total

Amazon's 2019 commitment was to reach "100% renewable energy by 2030".[^amz2019] Its current target reads "Match 100% of the electricity consumed by our global operations with renewable energy by 2025".[^amz2025]

Microsoft's 2020 pledge described "power purchase agreements for green energy contracted for 100 percent of carbon emitting electricity".[^ms2020] The 2026 milestone it announced was matching "100% of our annual global electricity consumption with renewable energy". Long-term contracts made up more than 90% of that, and grid-mix renewables counted toward the rest.[^msfeb]

All four companies now claim a 100% renewable match.[^gr2026][^amz2025][^meta2025][^msfeb] All four are annual, global totals. In plain terms: over the year, a company buys (or counts from the grid mix) as much renewable electricity as it uses, wherever and whenever that electricity was produced. Solar power bought at noon in one country can, on paper, cover a data centre running on gas at night in another. Google's own reports put that 100% annual match next to its 65% hourly carbon-free figure for the same year. That gap is why "100% renewable" and "carbon-free" are different claims.

### Carbon-neutral claims were discontinued

The accounting underneath all this matters, so a short primer. Scope 2 is the emissions from the electricity a company buys, and there are two ways to count it. Location-based applies the average emissions intensity of the grids where you consume electricity. Market-based applies the emission factors of the contracts and certificates you hold, so electricity covered by renewable certificates or contracts counts as zero and only the uncovered remainder is counted. Neither is a direct measurement, but location-based is the closer physical proxy.

The difference is large. From the companies' own latest tables, market-based Scope 2 sits 77% below location-based at Microsoft and 81% below at Google. At Meta it is more than 99.9% below: its data centres account for 135 tonnes market-based against 5.86 million tonnes location-based.[^msfs][^gr2026][^meta2025] Amazon does not publish a location-based figure in its report, so the gap cannot be computed.

Part of that gap has come from unbundled renewable energy certificates (RECs). A REC is a certificate that a unit of renewable electricity was generated somewhere. Unbundled means it was bought separately from any electricity actually delivered to you. Bloomberg calculated in 2024 that without them, Amazon's 2022 Scope 2 emissions would have risen by about 8.5 million tonnes, roughly three times what it reported. Microsoft's would have risen by about 3.3 million tonnes on a reported 288,000, an addition roughly 11 times the reported Scope 2 figure.[^bbg] Those multipliers apply to 2022 electricity emissions, not total footprints.

That is the backdrop to the most honest move of the period. In February 2025 Microsoft stopped buying spot-market unbundled certificates. Its market-based Scope 2 went from about 259,000 tonnes CO2e in its 2024 financial year to about 2.7 million in its 2025 financial year, driven by that change and by data centre growth. It wrote that the change "may temporarily move us out of a carbon-neutral position" for parts of its footprint, adding "we have discontinued reporting on our carbon neutrality and percentage of renewable electricity metrics."[^msfs] A worse-looking number produced by better accounting deserves credit. It also shows how much of the earlier picture was certificates, not atmosphere.

## Who wants the rules to change

The GHG Protocol is revising its Scope 2 guidance, and the central proposal was to require hourly matching from deliverable grid regions. The consultation closed in January 2026 with nearly 1,100 responses and "low support for hourly matching and deliverability as proposed", lowest among companies and industry groups.[^ghgp] In July 2026 the Independent Standards Board asked for further work on "multiple market-based method reporting approaches". Nothing is final, and the 2015 guidance still applies.

According to InfluenceMap, Google publicly supported the update.[^im] Amazon and Meta did not respond publicly in their own names. Both belong to the Emissions First Partnership, which opposed "mandatory hourly or deliverable matching" in favour of counting avoided emissions wherever clean power is bought. Microsoft took no public position we could find.

Both sides have a commercial interest. Hourly matching suits Google's 24/7 strategy. The avoided-emissions argument, that money spent on dirtier grids displaces more carbon, is a real argument in the literature as well as a convenient one.

## "AI will help solve it"

Alongside the rising numbers runs a second narrative. Google and BCG wrote in 2023 that AI "has the potential to help mitigate 5-10% of global greenhouse gas (GHG) emissions by 2030", a projection from a consultancy report, not a measurement.[^gbcg][^kjhoax] Microsoft called AI "an essential tool to accelerate progress toward sustainability".[^msai] Google's 2026 report announcement estimates that nine of its products helped others reduce about 41 million tonnes, "roughly three times Google's own emissions".[^gblog2026][^kjgoogle]

Maybe. But enabled or avoided emissions are counterfactual estimates with no agreed standard, and they cannot be subtracted from an emissions inventory. However large the estimate:

<p class="pull-quote">A tonne someone else might not have emitted is not a tonne you did not emit.</p>

## Why this is your problem too

Scope 3 covers the emissions in everything a company buys and uses, and if you buy cloud compute or AI services, your share of your provider's emissions belongs in your own Scope 3, under purchased goods and services. Many teams take that share from the provider's own carbon footprint tool, which often reports market-based figures. Whatever the provider's accounting choices make disappear then also disappears from your report. It is the blind spot we covered in [Your GHG report is lying to you](/blog/2026-02-13-ghg-problem/).

Regulation is moving, slowly. The [AI Act](/blog/2026-02-06-ai-act/) requires providers of general-purpose AI models to document the known or estimated energy consumption of their models. That documentation goes to regulators rather than the public, and it does not settle how to count what a data centre emits. And carbon is only one of the footprints at stake, as we argued in our post on [carbon, water and land tradeoffs](/blog/2026-09-28-carbon-water-land-tradeoffs/).

So when a vendor tells you its AI runs on 100% renewable energy, ask three questions. Is that annual or hourly matching? What are your location-based emissions? What changed in your methodology since last year?

## Our view

A pledge is a sentence, and sentences can be reworded. An inventory is a commitment to keep publishing the uncomfortable number. The most credible thing any of these four companies did in the last two years was not a new target. It was Microsoft dropping a certificate habit and reporting the jump, and Google publishing its 65% hourly figure next to its 100% annual one.

That holds at every scale. A plain, honest account of what your software actually consumes, using a method you do not change when the numbers turn against you, is worth more than a polished 2030 promise. If you want help building that kind of account, [get in touch](/contact/). If you want independent verification of the organisational and engineering practices behind it, rather than of the pledge, that is what [GSP™](https://gsp.greenseal.dev/) is for.

### Further reading

Ketan Joshi has written extensively in the same space, from Big Tech's selective disclosure to "AI for climate" claims. Readers who want to go deeper may find his work useful.[^kjselective][^kjhoax][^kjgoogle][^kjmoon]

*Updated 13 October 2026 to add further reading.*

### A note on AI use

We used AI (Claude, through Claude Code) to help analyse the companies' reports, find sources and refine drafts. The analysis and the conclusions are the author's, and so is the responsibility for any errors. We estimate the AI work used roughly 0.7 to 2.5 kWh of electricity, most likely around 1 kWh, based on token counts with our open-source tool [pegada](https://github.com/GreenSeal-dev/pegada-code).

[^ms2020]: Brad Smith. "Microsoft will be carbon negative by 2030". Official Microsoft Blog, 16 January 2020. [https://blogs.microsoft.com/blog/2020/01/16/microsoft-will-be-carbon-negative-by-2030/](https://blogs.microsoft.com/blog/2020/01/16/microsoft-will-be-carbon-negative-by-2030/)
[^g2020]: Sundar Pichai. "Our third decade of climate action: Realizing a carbon-free future". Google, 14 September 2020. [https://blog.google/outreach-initiatives/sustainability/our-third-decade-climate-action-realizing-carbon-free-future/](https://blog.google/outreach-initiatives/sustainability/our-third-decade-climate-action-realizing-carbon-free-future/)
[^amz2019]: Amazon. "Amazon Co-founds The Climate Pledge, Setting Goal to Meet the Paris Agreement 10 Years Early". 19 September 2019. [https://press.aboutamazon.com/2019/9/amazon-co-founds-the-climate-pledge-setting-goal-to-meet-the-paris-agreement-10-years-early](https://press.aboutamazon.com/2019/9/amazon-co-founds-the-climate-pledge-setting-goal-to-meet-the-paris-agreement-10-years-early)
[^meta2021]: Facebook. Renewable energy fact sheet, April 2021. [https://sustainability.fb.com/wp-content/uploads/2021/04/Facebook_RenewableEnergy_April2021.pdf](https://sustainability.fb.com/wp-content/uploads/2021/04/Facebook_RenewableEnergy_April2021.pdf). Current wording: [https://sustainability.atmeta.com/climate/](https://sustainability.atmeta.com/climate/)
[^gblog2026]: Kate Brandt. Google 2026 Environmental Report announcement, 30 June 2026. [https://blog.google/company-news/outreach-and-initiatives/sustainability/2026-environmental-report/](https://blog.google/company-news/outreach-and-initiatives/sustainability/2026-environmental-report/)
[^smith]: Akshat Rathi and Dina Bass. "Microsoft's AI Push Imperils Climate Goal as Carbon Emissions Jump 30%". Bloomberg Green, May 2024, as republished by the Taipei Times, 20 May 2024. [https://www.taipeitimes.com/News/editorials/archives/2024/05/20/2003818108](https://www.taipeitimes.com/News/editorials/archives/2024/05/20/2003818108)
[^msfs]: Microsoft. 2026 Environmental Data Fact Sheet, Tables 1A, 1B and notes. [PDF](https://cdn-dynmedia-1.microsoft.com/is/content/microsoftcorp/microsoft/msc/documents/presentations/CSR/2026-Microsoft-Environmental-Data-Fact-Sheet-PDF.pdf)
[^gr2026]: Google. 2026 Environmental Report. [https://sustainability.google/files/google-2026-environmental-report](https://sustainability.google/files/google-2026-environmental-report)
[^amz2025]: Amazon. 2025 Sustainability Report, including the letter from Kara Hurst and the 2019 to 2025 carbon footprint table. [PDF](https://sustainability.aboutamazon.com/2025-amazon-sustainability-report.pdf)
[^meta2025]: Meta. 2025 Environmental Data Index (calendar 2024 data). [PDF](https://sustainability.atmeta.com/wp-content/uploads/2025/10/Meta_2025-Environmental-Data-Index.pdf)
[^ms2024]: Microsoft On the Issues blog, 2024 Environmental Sustainability Report, 15 May 2024. [https://blogs.microsoft.com/on-the-issues/2024/05/15/microsoft-environmental-sustainability-report-2024/](https://blogs.microsoft.com/on-the-issues/2024/05/15/microsoft-environmental-sustainability-report-2024/)
[^ms2025]: Microsoft On the Issues blog, 2025 Environmental Sustainability Report, 29 May 2025. [https://blogs.microsoft.com/on-the-issues/2025/05/29/environmental-sustainability-report/](https://blogs.microsoft.com/on-the-issues/2025/05/29/environmental-sustainability-report/)
[^ms2026]: Brad Smith and Melanie Nakagawa. "Responsibly building the AI future", 9 July 2026. [https://blogs.microsoft.com/on-the-issues/2026/07/09/responsibly-building-the-ai-future/](https://blogs.microsoft.com/on-the-issues/2026/07/09/responsibly-building-the-ai-future/)
[^nco]: Canada's National Observer, 4 September 2025. [https://www.nationalobserver.com/2025/09/04/investigations/google-net-zero-sustainability](https://www.nationalobserver.com/2025/09/04/investigations/google-net-zero-sustainability)
[^kjmoon]: Ketan Joshi. "The life and death of Microsoft's moonshot", 31 May 2025. [https://ketanjoshi.co/2025/05/31/the-life-and-death-of-microsofts-moonshot/](https://ketanjoshi.co/2025/05/31/the-life-and-death-of-microsofts-moonshot/)
[^kjhoax]: Ketan Joshi. *The AI climate hoax*, with Friends of the Earth U.S., Beyond Fossil Fuels, Stand.earth, Climate Action Against Disinformation, Green Screen Coalition and Green Web Foundation, February 2026. [https://ketanjoshi.co/2026/02/17/big-tech-greenwashing-report/](https://ketanjoshi.co/2026/02/17/big-tech-greenwashing-report/), [PDF](https://foe.org/wp-content/uploads/2026/02/AI-for-climate-claims-Report_FEB-2026_FINAL.pdf)
[^kjgoogle]: Ketan Joshi. "Google's exponential path to climate-wrecking digital bloat", 1 July 2026. [https://ketanjoshi.co/2026/07/01/googles-exponential-path-to-climate-wrecking-digital-bloat/](https://ketanjoshi.co/2026/07/01/googles-exponential-path-to-climate-wrecking-digital-bloat/)
[^kjselective]: Ketan Joshi. "Big Tech's selective disclosure masks AI's real climate impact", 23 August 2025. [https://ketanjoshi.co/2025/08/23/big-techs-selective-disclosure-masks-ais-real-climate-impact/](https://ketanjoshi.co/2025/08/23/big-techs-selective-disclosure-masks-ais-real-climate-impact/)
[^gr2024]: Google. 2024 Environmental Report. [PDF](https://www.gstatic.com/gumdrop/sustainability/google-2024-environmental-report.pdf)
[^msfeb]: Melanie Nakagawa and Noelle Walsh. Official Microsoft Blog, 18 February 2026. [https://blogs.microsoft.com/blog/2026/02/18/a-milestone-achievement-in-our-journey-to-carbon-negative/](https://blogs.microsoft.com/blog/2026/02/18/a-milestone-achievement-in-our-journey-to-carbon-negative/)
[^bbg]: Akshat Rathi and Natasha White. "AI Tech Giants Hide Dirty Energy With Outdated Carbon Accounting Rules". Bloomberg, 21 August 2024. [Bloomberg](https://www.bloomberg.com/news/articles/2024-08-21/ai-tech-giants-hide-dirty-energy-with-outdated-carbon-accounting-rules), [syndicated copy](https://www.irishexaminer.com/business/companies/arid-41460145.html)
[^ghgp]: GHG Protocol. Scope 2 guidance revision and consultation, [https://ghgprotocol.org/scope-2-guidance](https://ghgprotocol.org/scope-2-guidance); Summary of public consultation feedback, 29 July 2026, [PDF](https://ghgprotocol.org/sites/default/files/2026-07/S2-ExecutiveSummary-PublicConsultation%20ummaryofFeedback-2026.07.29.pdf)
[^im]: InfluenceMap. "Corporate Engagement on the GHG Protocol Scope 2 Consultation", 28 August 2026. [https://influencemap.org/insight/Corporate-Engagement-on-the-GHG-Protocol-Scope-2-Consultation-39494](https://influencemap.org/insight/Corporate-Engagement-on-the-GHG-Protocol-Scope-2-Consultation-39494)
[^gbcg]: Yossi Matias and Kate Brandt. Google, 20 November 2023. [https://blog.google/outreach-initiatives/sustainability/report-ai-sustainability-google-cop28/](https://blog.google/outreach-initiatives/sustainability/report-ai-sustainability-google-cop28/)
[^msai]: Brad Smith and Melanie Nakagawa. Microsoft On the Issues blog, 16 November 2023. [https://blogs.microsoft.com/on-the-issues/2023/11/16/accelerating-sustainability-ai-playbook/](https://blogs.microsoft.com/on-the-issues/2023/11/16/accelerating-sustainability-ai-playbook/)
