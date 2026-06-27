---
title: "From the Hugging Face Hub to robot hardware with Strands Agents and LeRobot"
url: "https://huggingface.co/blog/amazon/strands-lerobot-hub-to-hardware"
date: "2026-06-17"
author: "Sundar Raghavan and Cagatay Cali (Amazon)"
feed_url: "https://huggingface.co/blog/feed.xml"
---
This article shows how to integrate LeRobot with the Strands Robots SDK for an end-to-end robot learning workflow: record demonstrations on the Hugging Face Hub, train policies, test in MuJoCo simulation, and deploy to physical hardware by changing a single keyword argument. The workflow keeps LeRobot's dataset format consistent across simulation and the physical SO-101 robot, supports policy providers like GR00T and MolmoAct2, and coordinates multi-robot fleets via a Zenoh peer mesh.
