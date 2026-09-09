---
author: Abiola Lapite
title: Artemis II Launches
tags: 
    - programming
    - mathematics
    - llms
    - ai
categories: programming
---
It's been 5 months since I last made a blog entry, but it's not because I haven't had anything new to say. To the contrary, so much has been going on recently that I've constantly felt as if my time would be better spent dealing with whatever issue was most pressing in the moment than on writing articles hardly anyone was likely to read. 

While I'm still as busy as ever, going forward, I'll try to make a special effort to put my thoughts down in writing much more regularly, no matter how hectic things get. I'd like to get to the point where making a new entry is as habitual as having a cup of afternoon coffee, and the key to making a new habit stick is to be diligent in practicing it even when it feels inconvenient. 

With the preceding out of the way, this seems like a good time to revisit some of the assessments I made several months ago. One such assessment was that local LLM inference [made no financial sense](2025-11-05-running-large-language-models-locally.md) unless one were constrained by privacy considerations. That assessment has held up well over time, and in fact is more true today than it was at the time, thanks to the skyrocketing prices for RAM and SSD storage. 

While more and more powerful open-weight models have appeared on the scene (mostly thanks to the efforts of Chinese companies), they have also witnessed a ballooning in size, from 550 billion parameters with Nemotron 3 Ultra to 2.8 trillion parameters with Kimi K3; even a highly efficient model like Z.ai's GLM 5.3 still amounts to 750 billion parameters. Even 3-bit quantisations of such models aren't sufficient to bring them down into memory ranges available to most consumers, and that's without considering return on investment. Unless the hardware being used for local inference is under constant high utilisation, it makes a lot more sense to simply pay $100/month to OpenAI or Anthropic and enjoy constant access to the very best models - there's no guarantee that hardware sufficient to run a model like GLM 5.3 will still be up to handling whatever succeeds it in 6 months time. 

The sole justification I could see for using purely local inference was due to privacy concerns, but that doesn't mean the concern is a marginal one. As [we are](https://cims.nyu.edu/~tristanb/statement.pdf) currently [seeing](https://openai.com/index/navier-stokes-solution/) with the controversy around the Navier-Stokes problem, it isn't really obvious what guarantees companies OpenAI and Anthropic make about how they handle customer data. For example, while [OpenAI states](https://help.openai.com/en/articles/5722486-how-your-data-is-used-to-improve-model-performance) that they take steps to eliminate personal information when training on user queries, personal information is hardly the only type of information one might wish to keep private. Taking this statement at face value, there is nothing preventing OpenAI from using highly valuable data about a researcher's findings or a company's market strategy. Is this a risk most would find worth taking if they knew about it? How carefully are scientists, engineers, developers and management types thinking about the implications of all of this, in the heedless rush to adopt "AI" for fear of being left behind by the competition? What's to stop the company you're serving your internal data to on a platter from using that same data to train new models which will eat your lunch tomorrow?   