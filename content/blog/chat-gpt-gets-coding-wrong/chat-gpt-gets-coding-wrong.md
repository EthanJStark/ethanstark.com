---
title: ChatGPT Bad At Coding? A Closer Look
description: Thinking critically about breathless headlines
date: 2023-08-06
tags:
  - ChatGPT
  - media literacy 
  - LLM
  - coding
---

There's an article making the rounds. [ChatGPT's odds of getting code questions correct are worse than a coin flip](https://www.theregister.com/2023/08/07/chatgpt_stack_overflow_ai/)! it breathlessly proclaims. 

Let's take a closer look at the source study it cites.

A pre-print study titled **Who Answers It Better? An In-Depth Analysis of ChatGPT and Stack Overflow Answers to Software Engineering Questions** [arxiv link](https://arxiv.org/abs/2308.02312) [pdf](https://arxiv.org/pdf/2308.02312)

First off: the study is not peer-reviewed. It's a pre-print, meaning it hasn't been reviewed by other experts in the field. It's also not published in a journal, but on arxiv, a site where researchers can post their work.

Second: any article that references "ChatGPT" without specifying if it's version 3.5 or 4 needs to be carfully examined. Sure enough, deep in the body of the study, it notes that they're using version 3.5. In my experience, 4 is much better at coding questions.

Lastly, and most critically: as software engineers, we do not simply expect a snippet of code to work, be it from Stack Overflow or generated from an LLM. We write automated tests to verify that the code works as expected. If an LLM can get me 90% of the way there, and I can debug the last bit, I'll take it!
