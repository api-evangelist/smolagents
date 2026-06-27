---
title: "Is it agentic enough? Benchmarking open models on your own tooling"
url: "https://huggingface.co/blog/is-it-agentic-enough"
date: "2026-06-18"
author: "Lysandre, Nathan Habib, Pedro Cuenca"
feed_url: "https://huggingface.co/blog/feed.xml"
---
This article introduces a benchmarking harness that evaluates how well open-source libraries work with AI coding agents, measuring not just correctness but the effort required in tokens used, time spent, and error rates across model sizes and library versions. Testing on the transformers library revealed that features helping large models could inadvertently confuse smaller ones, showing the importance of agent-optimized software design.
