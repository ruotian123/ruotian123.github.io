---
title: "Smart Traffic Signal Control in Urban Environments Leveraging SUMO and Curiosity-Enhanced MAPPO"
excerpt: "This paper proposes a pedestrian-aware, curiosity-enhanced MAPPO framework for urban multi-intersection traffic signal control, incorporating Random Network Distillation to improve exploration efficiency. Evaluated on a 16-intersection Helsinki traffic network in SUMO, the method accelerates convergence and improves queue length, waiting time, throughput, and pedestrian service quality compared with vanilla MAPPO and representative baselines.<br/><img src='/images/portfolio_RND_MAPPO_1.jpg'>"
collection: portfolio
---

<img src='/images/portfolio_RND_MAPPO_1.jpg'>

Project Type: Research Project<br/>
Duration: March 2023.09 – 2024.06  
Role: Lead Researcher  
Keywords: Reinforcement Learning, Traffic Signal Control, Multi-agent Reinforcement Learning, Curiosity Mechanism
## TL;DR

We develop a pedestrian-aware multi-agent traffic signal control framework that integrates Random Network Distillation with MAPPO. Curiosity-driven exploration enables the intersection agents to learn coordinated signal control policies more efficiently in a realistic Helsinki traffic network.

## Motivation

Urban multi-intersection traffic signal control is challenging because the effects of signal decisions are delayed, neighboring intersections are strongly coupled, and pedestrian service requirements may conflict with vehicle throughput. Existing multi-agent reinforcement learning methods primarily focus on coordination architectures, while exploration efficiency during training has received comparatively less attention.

## Method

We formulate pedestrian-aware traffic signal control as a cooperative multi-agent reinforcement learning problem. Each signalized intersection acts as an agent and executes a decentralized policy based on its local traffic observation.

The proposed method uses MAPPO as the cooperative learning backbone and incorporates Random Network Distillation as an intrinsic-reward mechanism. The RND module encourages each agent to visit less familiar traffic states during training, while the extrinsic reward maintains the vehicle and pedestrian traffic-control objectives.
