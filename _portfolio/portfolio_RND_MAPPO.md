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
<img src='/images/portfolio_RND_MAPPO_5.jpg'>

## Experimental Setting

The method is evaluated in SUMO on a real-map-based Helsinki traffic subnetwork containing 16 signalized intersections. The environment includes both vehicle and pedestrian traffic and is evaluated under low-, medium-, and high-demand conditions.

## Key Results

Compared with vanilla MAPPO, the proposed RND-MAPPO method achieves:

- **26.96% reduction** in average queue length;
- **35.30% reduction** in average vehicle waiting time;
- **11.88% improvement** in throughput;
- **36.43% reduction** in average pedestrian waiting time;
- **21.0% improvement** in the area under the learning curve;
- **38.3% reduction** in the number of episodes required to reach the predefined performance threshold.

## My Role

I led the project investigation and implementation and wrote the original manuscript draft.

## Abstract

In urban multi-intersection traffic signal control, learning effective policies is challenging because signal decisions have delayed effects, intersections are strongly coupled, and pedestrian service requirements may conflict with vehicle throughput. While multi-agent reinforcement learning provides a promising framework for coordinated signal control, most existing studies primarily emphasize inter-agent coordination and pay limited attention to exploration efficiency during training. To address this issue, this paper proposes a pedestrian-aware curiosity-enhanced Multi-Agent Proximal Policy Optimization (MAPPO) method for urban traffic signal control, in which Random Network Distillation (RND) is incorporated as an intrinsic-reward mechanism to encourage more effective exploration. The proposed method is evaluated in SUMO on a real-map-based Helsinki traffic network with 16 signalized intersections and is compared with vanilla MAPPO and several representative traffic signal control baselines. Experimental results show that the proposed method not only accelerates training convergence but also improves key traffic performance metrics, including queue length, waiting time, throughput, and pedestrian service quality. These results demonstrate the effectiveness of curiosity-driven exploration for multi-agent traffic signal control in realistic urban environments.
