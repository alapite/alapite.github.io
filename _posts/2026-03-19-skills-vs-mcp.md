---
author: Abiola Lapite
title: Skills or MCP?
tags:
    - Large Language Models
    - Machine Learning
    - Programming
categories: programming
---
It's been only a few months since Anthropic introduced the [Model Context Protocol](https://modelcontextprotocol.io/), and suddenly it seemed every developer was busy working on their own MCP server implementations. However, even as the hype around MCP was still building, Anthropic then announced its [Agent Skills](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview) approach, which seemed to cover much of the same use cases, but in a less heavyweight manner. Suddenly MCP came to look dead in the water, especially given its tendency to bloat the limited context windows of even the most capable agents. Skills, when properly structured, are much more lightweight, with only their descriptions needing to be initially loaded into the context, and the reading of any further data being deferred until actually necessary.

It's with the above in mind that I find [this Confluent Developer video](https://www.youtube.com/watch?v=pvxNcQTcIy4) so interesting. The video provides an insightful way of thinking about the MCP vs. Skills question, by phrasing it as a matter of static vs. dynamic data. Skills, by their nature, are largely static, describing processes and practices, while MCP is better suited to dynamic tasks like reading from a Kafka queue, fetching the latest weather report for a given location, etc. Of course, this distiction isn't a rigid one, as developers can give their skills the ability to call tools via the CLI, so it's not clear that MCP really is necessary, at least when writing code.

Where MCP **does** seem to maintain an advantage over Skills is with agentic tools of the sort popularised by OpenClaw and Claude Cowork. When building software around agents, one can't assume that one's intended userbase will have access to a CLI (e.g. due to corporate security policies prohibiting such access). While one could try to get around the CLI issue by simply embedding one in the software being deployed, one would hope most developers would be deferred by the possible security implications of doing so - but then again, OpenClaw is wildly popular despite all its issues ... 

In contrast, dedicated MCP servers can be highly restricted in their capabilities, and any MCP servers needed by a security-conscious agentic application can be bundled with the rest of the code being deployed, whether as standalone executables or as modules in a single monolithic application binary. 