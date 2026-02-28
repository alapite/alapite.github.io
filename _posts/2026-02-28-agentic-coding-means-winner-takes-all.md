---
author: Abiola Lapite
title: Agent-Driven Coding Means Winner Takes All 
tags:
- Large Language Models
- Machine Learning
- Open Source
- Programming
categories: programming
---

I recently ran into a [study on Claude Code](https://amplifying.ai/research/claude-code-picks/report) carried by Amplifying on which tools Anthropic's harness chooses when given free rein. According to the study, the strongest tendency was actually for Claude Code to reinvent the wheel[^1]. However, when Claude Code did pick an available library or framework, it tended to pick the same ones again and again (e.g. PostgreSQL, Tailwind CSS, Pytest). This was consistently the case across all three of Sonnet 4.5, Opus 4.5 and Opus 4.6.

Now, this result isn't really very surprising, as it likely reflects the distribution of actual tool usage in the training sets used to build these models. For any given language, one would expect a small set of tools to dominate usage, so, for example, in the Java world, the likeliest candidates for a backend service would be a combination of Spring Boot, Hibernate, JUnit 5, Mockito and Lombok. This isn't _necessarily_ a bad thing, as it's almost certainly the case that practitioners in a given field have converged on their preferred options for well-founded reasons. An agentic harness which defaults to the same choices is likely to be doing the right thing, unless one provides it with good reasons not to opt for said defaults.

If there's a problem with this tendency, it's that it tends to cement today's justifiable defaults as the unchanging winners going forward. As more and more publicly-availabe code is of the "vibe-coded" or "one-shotted" variety, they will constitute an ever larger share of the training data fed into the models of the future. Given the strong tendency of such model-generated code to use today's defaults (when they aren't busy reinventing the wheel), this will likely lead to a self-reinforcing cycle which ends with said defaults cemented in place forever, whatever the merits of any new alternatives which may come along.

I suppose one could make the argument that, just as hardly anyone cares about the nature of the machine code produced by interpreters or compilers any more, as long as said code meets performance and safety standards, it shouldn't really matter whether any particular libraries or frameworks become set in stone, as long as the coding agents which use them still turn out work that meets requirements. Who cares about how ugly [x86_64](https://en.wikipedia.org/wiki/X86-64) assembly is compared to its [ARM](https://en.wikipedia.org/wiki/AArch64) equivalent? 

My own counterpoint to this line of argument is that such things typically don't matter until they do. Going back to the Intel vs. ARM discussion, Intel **did** manage for a long time to overcome the many disadvantages of its CPU architecture through sheer weight of resources, beating back not just challengers like [DEC Alpha](https://en.wikipedia.org/wiki/DEC_Alpha), [SPARC](https://en.wikipedia.org/wiki/SPARC) and [PowerPC](https://en.wikipedia.org/wiki/PowerPC), but even its own [Itanium](https://en.wikipedia.org/wiki/Itanium) offering in the process. However, once smartphones took off and became the primary device used by the great majority of people, Intel's financial muscle ceased to matter much in the face of ARM's much more efficient power consumption, especially once ARM began to be adopted by companies with even more financial might than Intel.

It's easy to envisage a similar future for library and framework choices which have become ossified as mandatory due to the influence of agentic coding. New ways of approaching and solving problems might emerge which offer huge advantages over older ways of doing things, but of which most "AI first" developers might never become aware, as they lose touch with the underlying details of their work and leave the nitty-gritty to trusty old Claude. Perhaps this might provide the opening for the resurgence of more "old-school" (or, as some might call them, "diehard") types who still enjoy an intimate familiarity with lower-level tools? 

[^1]: A course of action software developers are generally advised to avoid, for very [good reasons](https://blog.67bricks.com/?p=783). 