---
author: Abiola Lapite
tags: llms
categories: machine-learning
---
In my [previous post](2025-11-10-local-inference-on-macbooks.md) I laid out some issues to keep in mind when deciding whether it is worth going to the trouble of running LLMs locally. As I tried to make clear, the answer in most cases is almost certainly "No". The answer is only clearly "Yes" when 
1. privacy considerations come into the picture, or 
2. one already owns the necessary hardware, which also has the needed software support.

At present, the largest pool of individuals for whom the second case applies will be those who own [M-Series Macs](https://en.wikipedia.org/wiki/Apple_silicon#M-series_SoCs) with sufficient amounts of RAM (i.e. 24 GB or more). It's certainly possible to try out running inference on machines with only 16 GB of RAM, but this will limit the possibilities to only very small models, as the same memory also has to accommodate the operating system and any other applications the user might be running.

### Machine Specs and Model Choice
The two primary factors determining what will be possible running LLMs on a Mac will be
1. How much RAM the machine has, and
2. How much memory bandwidth the system provides

Obviously, in both cases, the more, the better. Other factors do also matter, e.g. the number of GPU cores packaged on the machine's SoC, and their generation (with GPU performance jumping about 35% going from M4 to M5, for example). Still, these are second-order considerations, with the sheer amount of RAM and the speed of access to it being most important (though this well might change once M5-Pro and M5-Max machines are released next year). 