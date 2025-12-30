---
author: Abiola Lapite
tags:
- llms
- ai
- machine-learning
- macos
- macbook
categories: machine-learning
---
With Z.ai's recent release of its [GLM-4.7](https://z.ai/blog/glm-4.7) model, and the mostly uninformative responses to the company's recent [Reddit AMA](https://www.reddit.com/r/LocalLLaMA/comments/1ptxm3x/ama_with_zai_the_lab_behind_glm47/), the writing was in the air that the company had no more interest in catering to local inference by offering any updates to its (justifiably) popular [GLM 4.5 Air](https://z.ai/blog/glm-4.5), which offered most of the performance of the full GLM 4.5 model while requiring just 106 billion parameters (as opposed to GLM 4.5's 355 billion). Any doubts as to why Z.ai might have taken this direction were settled for me on learning that the company is [set to IPO](https://www.reddit.com/r/LocalLLaMA/comments/1pz68fz/z_ai_is_going_for_an_ipo_on_jan_8_and_set_to/) in Hong Kong on the 8th of January. The company needs to make money, and one clear way to do is by selling subscriptions to all of those who might otherwise have been tempted to host a GLM 4.7 Air on their local hardware.

Z.ai's shift in strategy is being aided by an astonishing rise in RAM prices in recent months, thanks to the ongoing GPU gold rush, which has incentivised the major RAM manufacturers to emphasise the production of HBM [at the expense](https://www.npr.org/2025/12/28/nx-s1-5656190/ai-chips-memory-prices-ram) of lower-margin DRAM. I've seen DDR5 prices listed recently for up to 4 times what they were going for just half a year ago, and there are indications of [even more price hikes](https://www.theverge.com/news/848199/ram-shortage-pc-phone-price-increases) up ahead. This development dramatically tilts the playing field in the favour of big players who have already built up their cloud infrastructure and/or have large amounts of funding to subsidise cloud-based subscription plans (at least for the moment). If local inference for cutting-edge models made little economic sense before, it makes absolutely **none** now, when [Z.ai is offering](https://z.ai/subscribe) a "Lite" plan with supposedly **3x** the usage limits of Claude Pro, at just $18/quarter.

In the near term, the only scenarios in which local inference can be justified will be those in which
1. Privacy guarantees are absolutely critical,
2. One already owns sufficiently capable hardware, which also happens to be relatively idle,
3. The intended use cases for LLMs are relatively narrow and well-defined ones for which small models can be made to work just fine.

For everything else, the subsidised cloud plans will have to do for now, at least until the AI hype dies down and hardware prices come back down to Earth. In the meantime, aggressive adopters of cloud-based services will have to keep a keen eye out to avoid getting too locked into any one provider. The subsidies all of these companies are currently offering will only last as long as investors retain patience for all the high-flying talk of imminent "AGI" and the pot of gold at the end of a rainbow which will come with it. 

A telling sign of where things are headed is Z.ai's refusal to offer plans with time-horizons longer than 3 months, no matter how much users might be willing to pay. If the company's imminent IPO goes through as planned, Z.ai will need to regularly demonstrate to investors that it has a viable roadmap to profitability, which means it will need to raise prices enough for all that subscription revenue to service not just the hardware and hosting costs for all of the customer model usage, but also the prior R&D costs sunk into getting to GLM 4.7, **and** the ongoing costs of the R&D required to keep it abreast of competitors' advances. Given that Anthropic is still losing money while charging **16 times more** than Z.ai for **1/3** of the usage, I expect Z.ai's first takers to be in for a rude awakening over the next few months.    