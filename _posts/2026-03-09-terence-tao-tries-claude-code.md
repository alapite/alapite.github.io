---
author: Abiola Lapite
title: Terence Tao Tries Claude Code
mathjax: true
tags: 
  - Lean
  - Mathematics
  - Large Language Models
  - Machine Learning
  - Programming
categories: mathematics
---

The last few weeks have seen a series of headline-grabbing announcements about "AI" models supposedly making big strides in their mathematical capabilities, not least of which was Google's [announcement](https://deepmind.google/blog/accelerating-mathematical-and-scientific-discovery-with-gemini-deep-think/) of its "Aletheia" math research agent. Built on [Gemini 3 Deep Think](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-deep-think/), Aletheia is claimed to go beyond just *"AI-guided collaboration"* to *"reliable autonomous research"*. 

Meanwhile, OpenAI [shared a post](https://openai.com/index/first-proof-submissions/) outlining their attempts at the ["First Proof" challenge](https://1stproof.org/), an effort at providing a more meaningful challenge of the abilities of "AI" models by drawing up 10 math questions unlikely to be solvable simply by exhaustively trawling through all of the existing literature. If OpenAI is to be believed, their model is likely to have solved at least 5 of the 10 First Proof problems, though [initial feedback](https://www.reddit.com/r/math/comments/1r4gpi5/first_proof_solutions_and_comments_attempts_by/) from experts suggests OpenAI's claims are likely exaggerated.     

Hot on the heels of the "Aletheia" announcement came news [from Math, Inc.](https://www.math.inc/sphere-packing) about the success of their "Gauss" agent in auto-formalising Maryna Viazovska's proof of the [Sphere Packing problem](https://en.wikipedia.org/wiki/Sphere_packing) in 8 and 24 dimensions. This 200,000-line proof was supposed to have taken Gauss just 3 weeks to put together.

With reports like these following each other in rapid succession, it's interesting to see what an actual working mathematician like Terence Tao[^1] [makes of his experience](https://youtu.be/JHEO7cplfk8) working with a frontier model and harness like Claude Code and Opus 4.6. In this video, Tao doesn't attempt to use Claude Code to derive new insights, but to formalise a proof that already exists in the "informal" (aka human-readable) guise mathematicians are used to dealing with.

As Tao's video illustrates, the line between writing software and crafting a mathematical proof really is a blurry one, even in a real-world context like trying to formalise a proof in Lean. Most of the hype around Claude has mostly been about its software development capabilities, so one might imagine this work would be a piece of cake for Anthropic's agent, but that turns out to be far from the case. At the start of the video, Tao explains how he started off trying to "one shot" the whole process by simply handing the informal proof over to Claude Code, and asking it to create a formalised version. The result of this initial attempt, after lots of churning and much token-consumption, turned out to be less than satisfactory. 

Tao then decided to adopt a strategy which most software developers quickly converge on, after a little experience with tools like Claude Code: divide the problem into smaller chunks, then, in an iterative process, have the agent work on each chunk, verify that the result is in line with what was requested, and only **then** do you proceed to the next chunk of work. The "one shot" approach is great as a sales gimmick, but when you need your work to be 100% correct, being able to quickly prompt your way to 90% of your goal is pointless if that last 10% remains perpetually out of reach. Research mathematics just happens to be all about 100% correctness.

Something else noteworthy about Tao's Claude Code experience was how the agent failed to spot obvious opportunities for refactoring that Tao noted. When I say "obvious" here, I don't mean it in that condescending way one sometimes sees in mathematics textbooks[^2], but in the _"this code is a near exact duplicate of the code above"_ way simple enough for IDEs to spot even in the days before "AI" became a buzzword. One doesn't need to understand any of the mathematics the agent is trying to formalise to see the issue Tao was pointing out, so it was surprising Claude Code failed to catch the redundancy, given the fervour with which so many promote its abilities online.

While I suggest watching the video oneself and drawing one's own conclusions, what I take away from it is that one should take with hearty pinches of salt all of the claims from Anthropic, Google and OpenAI about the advances they are making in mathematics. These tools are almost certainly more proficient at applying well-understood techniques better than the vast majority of people, so if you need to deal with some tricky but well-studied differential equation, or some other such problem with lots of prior art, you likely will benefit from using today's frontier models. This will also likely be true even for research mathematicians, who may need to carry out straightforward but tedious tasks to establish a result of greater interest[^3]. What even the best models **won't** be doing in the next 12 months is coming up with genuinely new and interesting mathematical ideas.

[^1]: A [Fields Medalist](https://en.wikipedia.org/wiki/Fields_Medal), no less.
[^2]: Notably, the tendency for textbook authors to declare proofs as "obvious" because they can't be bothered to spell things out for their audience, to whom it may be anything but "obvious" (otherwise they probably wouldn't need said books to begin with).
[^3]: As in the case of the computer-generated proof of the [4-Colour Theorem](https://en.wikipedia.org/wiki/Four_color_theorem).