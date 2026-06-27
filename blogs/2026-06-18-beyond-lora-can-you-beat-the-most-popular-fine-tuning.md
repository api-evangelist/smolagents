---
title: "Beyond LoRA: Can you beat the most popular fine-tuning technique?"
url: "https://huggingface.co/blog/peft-beyond-lora"
date: "2026-06-18"
author: "Benjamin Bossan, Sayak Paul, Marian, Kashif Rasul"
feed_url: "https://huggingface.co/blog/feed.xml"
---
The article challenges the assumption that LoRA is the universally optimal parameter-efficient fine-tuning (PEFT) approach, noting it appears in 98.4% of Hugging Face model cards mentioning a single PEFT technique. Benchmarking with the PEFT library shows alternatives can win on specific axes: OFT achieved better image-generation results with more memory efficiency, while Lily outperformed LoRA on mathematical reasoning accuracy at the cost of more memory.
