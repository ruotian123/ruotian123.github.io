---
title: "Smart Traffic Signal Control in Urban Environments Leveraging SUMO and Curiosity-Enhanced MAPPO"
collection: publications
category: manuscripts
permalink: /publication/2026-06-15-paper_RND_MAPPO
excerpt: 'This paper proposes a pedestrian-aware, curiosity-enhanced MAPPO framework for urban multi-intersection traffic signal control, incorporating Random Network Distillation to improve exploration efficiency. Evaluated on a 16-intersection Helsinki traffic network in SUMO, the method accelerates convergence and improves queue length, waiting time, throughput, and pedestrian service quality compared with vanilla MAPPO and representative baselines.'
date: 2026-05-15
venue: 'IET Intelligent Transport System'
paperurl: 'https://ruotian123.github.io/files/paper_RND_MAPPO1.pdf'
bibtexurl: 'https://ruotian123.github.io/files/bibtex_RND_MAPPO.bib'
citation: 'Chen, R., Tang, X., Ruotsalainen, L., Yan, Z., & Zhou, C. (2026). Smart Traffic Signal Control in Urban Environments Leveraging SUMO and Curiosity‐Enhanced MAPPO. IET Intelligent Transport Systems, 20(1), e70247.'
---
In urban multi-intersection traffic signal control, learning effective policies is challenging because signal decisions have delayed effects, intersections are strongly coupled, and pedestrian service requirements may conflict with vehicle throughput. While multi-agent reinforcement learning provides a promising framework for coordinated signal control, most existing studies primarily emphasize inter-agent coordination and pay limited attention to exploration efficiency during training. To address this issue, this paper proposes a pedestrian-aware curiosity-enhanced Multi-Agent Proximal Policy Optimization (MAPPO) method for urban traffic signal control, in which Random Network Distillation (RND) is incorporated as an intrinsic-reward mechanism to encourage more effective exploration. The proposed method is evaluated in SUMO on a real-map-based Helsinki traffic network with 16 signalized intersections and is compared with vanilla MAPPO and several representative traffic signal control baselines. Experimental results show that the proposed method not only accelerates training convergence but also improves key traffic performance metrics, including queue length, waiting time, throughput, and pedestrian service quality. These results demonstrate the effectiveness of curiosity-driven exploration for multi-agent traffic signal control in realistic urban environments.
