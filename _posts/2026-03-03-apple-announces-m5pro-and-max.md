---
author: Abiola Lapite
title: Apple Finally Announces the M5 Pro and M5 Max MacBook Pros 
tags: 
  - apple
  - hardware
  - llms
  - ai
  - machine-learning
categories: machine-learning
---
Ever since Apple [announced the base M5 MacBook Pro](https://www.apple.com/newsroom/2025/10/apple-unveils-new-14-inch-macbook-pro-powered-by-the-m5-chip/) back in October
last year, many with an interest in local LLM inference have been awaiting expectantly the release of the M5 versions of the higher-end MacBook Pros. The base M5 machine brought improvements over its predecessor which suggested that the M5 Pro and Max versions would be even better options for local inference than the M4 generation had already proven itself to be. Chief amongst these improvements were 
1. 27.5% more memory bandwidth, at 153 GB/s (as opposed to 120 GB/s for M4), and
2. tweaks to the neural accelerators, which promised up to 4x faster pre-fill performance (and at least one benchmarker [observing a 3.65x boost](https://www.reddit.com/r/LocalLLaMA/comments/1ocousf/m5_using_neural_accelerators_in_the_gpu_is_up_to/) in practice).

The improvement to pre-fill performance was particularly noteworthy because "time to first token" had been the biggest weakness of Apple Silicon to date, one which this particular improvement would do a great deal to address. The hope was that the M5 Pro and M5 Max machines, whenever they did come out, would enjoy similar boosts, making them even more attractive in an era when Nvidia and AMD have both essentially given up on the consumer GPU market, while skyrocketing memory and SSD prices make Apple's offerings seem ever more reasonable by comparison.

Now, the long-awaited machines are [finally here](https://www.apple.com/newsroom/2026/03/apple-debuts-m5-pro-and-m5-max-to-supercharge-the-most-demanding-pro-workflows/), and while both of the M5 Pro and M5 Max bring improvements in the two aforementioned areas, they aren't exactly what many had been hoping for, in at least one respect. 

The main thing worth noting is that both the Pro and Max chipsets get the same 12.5% bump in bandwidth percentage-wise, with the Pro chipset going from 273 GB/s to 307 GB/s, and the Max chipset going from 546 GB/s to 614 GB/s. Had the hopes borne of the M5's changes borne out, the bandwidth improvements would have been at least twice as big as they actually are, bringing the M5 Max that much closer to touching distance of the M3 Ultra's 819 GB/s.

I can understand why some may feel disappointed, but these numbers, when considered on their own terms, are actually class-leading, especially for the amount of RAM they make accessible. The maximum amount of RAM a consumer can get on a single NVIDIA card is 96 GB on the RTX PRO 6000, and while this card does enjoy a hefty 1.8 TB/s of bandwidth, it also costs northwards of £7,500 in the UK. Meanwhile, an M5 Max MacBook Pro with 128GB can [be pre-ordered](https://www.apple.com/uk/shop/buy-mac/macbook-pro) for £5,400 as a fully-functioning, highly power-efficient system, not just a single power-hungry card still in need of a motherboard, CPU, system memory, storage and - last but not least - a beefy PSU to power all of that hardware. Above all else, one can count on Apple's machines to actually be available to buy (and to be delivered within a month of ordering), while NVIDIA's RTX PRO 6000 seems likely to remain sold-out for the foreseeable future.   

Having sung the praises of Apple's new hardware, what practical consequences do I think one can draw from their coming on the market? While I think these updates will prove a hit for Apple, especially the 128GB M5 Max version, I don't see this news as altering the calculus for anyone other than those with strict privacy requirements which preclude the use of public APIs, or affluent enthusiasts with lots of discretionary income to spare. 

The harsh reality is that 128GB simply isn't enough to run anything close to the leading edge locally, anyone wanting the best results from coding agents is stuck paying Anthropic, OpenAI or Chinese alternatives like DeepSeek and Z.AI. For experimenting with smaller models like the recently released [Qwen 3.5](https://qwen.ai/blog?id=qwen3.5), older M3 and M4 class machines should still be usable, and these older MacBooks remain more than capable of handling most other tasks, making it hard to justify updating just for the inference improvements the new M5 machines offer. 

The story _might_ have been slightly different if Apple had offered the M5 Max MacBook Pro with 256GB of RAM, but even in that case I think only rich enthusiasts and the privacy-focused could justify spending whatever Apple would be willing to charge for such a configuration. To the extent a market exists for such higher-end configurations, it will have to wait for an M5 Ultra update for the Mac Studio before it is addressed. 