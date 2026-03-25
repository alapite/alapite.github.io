---
author: Abiola Lapite
title: Here Comes the Agentic Rug-Pull
tags:
    - ai
    - business
    - llms
    - machine-learning
    - programming
categories: programming
---
When I wrote about "Open" vs Local LLMs back in January, one of the possible issues I mentioned with going the subscription route was that the pricing strategy being adopted by all of the vendors would likely prove unsustainable, given the need to both recover previous training and research costs, as well as inevitability of all of these companies needing to keep spending heavily to keep abreast of their competitors. 

The relatively low subscription prices being offered by the likes of Anthropic and OpenAI for even their top-tier offerings is almost certainly well below what it would take to cover all of the costs these companies have incurred, are currently incurring, and will continue to incur. What developers are currently benefiting from is investor-largesse rooted in the same _"offer the first hit for free"_ logic beloved of drug-dealers everywhere. The hope is that enough businesses become sufficiently dependent on these "agentic coding" tools that when the inevitable price increases and service degradations begin, the customers are so far gone in their dependency that they can do little but grumble and accept whatever new terms are put before them.     

Back in January, I thought this dynamic would first be visible with less well-capitalised outfuts like Z.ai, which was so eager to go public to raise relatively little money. I expected that the big American firms like Anthropic and OpenAI would have a lot more leeway in how quickly they'd need to start scaling back on their generousity, given how much more funding they'd received than the Chinese competition. Z.ai's subsequent abrupt shift in subscription strategy and its inability to reliably serve its GLM-5 model[^1] have proven very much in line with what I'd expected to happen, but what I didn't count on was that both Anthropic and OpenAI would start following the same playbook so quickly. 

While neither of the American companies has suddenly started asking customers to pay a lot more, it's clear both from the many complaints on Reddit and from personal experience[^2] that they are both trying to rein in their costs in two ways: 
1. By making the same usage count much more severely against customer quotas[^3],
2. By tweaking the manner in which the models were being served[^4], so that the models suddenly seemed a lot less capable than they had been.

What's striking about what I've personally experienced with OpenAI's Codex is that this sudden change in the terms of service has occurred **within** what was supposed to be a "2X" window lasting up until the 2nd of April. If this is how bad things already are under such "generous" circumstances, once the "2X" promotion comes to an end, my Codex Plus subscription is likely to become as useless as Anthropic's "Claude Pro" limits already are (which is why I opted for Codex in the first place).

While there is a certain inevitability to what these companies are doing, the secretive manner in which they are going about it feels dishonest and disrespectful of their users. Rather than be upfront about their need to start reining in their losses as they seek to go public in the next few months, both Anthropic and OpenAI prefer to pretend that nothing has changed, and that any customers who insist otherwise are simply deluded, no matter how clearcut the evidence they base their complaints on. 

This "brush customer complaints aside" approach makes a certain cynical sense, given the need to keep the hype going until IPO time, as publicly acknowledging cost-cutting measures would fly in the face of the narrative that the big "agentic AI" vendors are already cash-flow positive, and are destined to soon turn into profit-gushing machines which will make the likes of Apple and Google envious. Why nickel-and-dime paying customers over an offering that is supposedly enjoying 80% profit margins, as the most gullible AI-boosters would have everyone else believe?

The harsh reality that commenters like Ed Zitron understand (while his many, supposedly more tech-savvy detractors do not), is that pretending that companies simply cannot ignore the cost of their capital outlays while pretending that all that matters is the operating margin of offering services on lots of costly hardware they didn't get for free. For Anthropic, OpenAI and others like them to be profitable under the [GAAP principles](https://en.wikipedia.org/wiki/Generally_Accepted_Accounting_Principles_(United_States)) which legally bind public companies with mandatory filing obligations, said **must** account for capital expenditures when calculating profit, and they must do so while making realistic assumptions about how quickly past capital expenditures will depreciate. In other words, they can't get away with pretending that all those costly GPUs will last for more than a few years before needing to be replaced with lots of even more expensive GPUs.

I believe that the lesson businesses and individual developers ought to draw from all of this is to either 
1. be ready to soon start paying many times more than they currently do for what they're getting,
2. be willing to incur huge sums upfront to host their own fine-tuned versions of open-weight models in-house, or
3. refrain from plunging wholesale into the whole "agent-driven development" approach, by keeping developers central to the actual process of writing code, even if occasionally calling on LLM assistance. 

[^1]: Even at the new and much higher prices the company is demanding of subscribers.
[^2]: In my case, with Codex Plus, which took a sudden and drastic turn for the worse starting on the 13th of March.
[^3]: For example, after several weeks of my Codex allowance never falling more than 15% in a day, I suddenly saw 45% disappear in the space of one afternoon, despite doing nothing particularly fancy or unusual.
[^4]: E.g. by extreme quantisation of model weights.