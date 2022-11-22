---
title: "Robotic Table Wiping via Reinforcement Learning and Whole-body Trajectory Optimization"
collection: publications
permalink: /publication/table_wiping
excerpt: '<br />
[Project Page](/publication/table_wiping) / 
[Paper](https://arxiv.org/abs/2210.10865) / 
[Video](https://www.youtube.com/watch?v=inORKP4F3EI&feature=youtu.be)
- We propose an effective strategy for table wiping combining the strengths of reinforcement learning and whole-body trajectory optimization.'
date: 2022-10-19
venue: 'Under Review'
# venuetype: "journal"
paperauthors: 'T. Lew, S. Singh, M. Prats, J. Bingham, J. Weisz, B. Holson, X. Zhang, V. Sindhwani, Y. Lu, F. Xia, P. Xu, T. Zhang, J. Tan, M. Gonzalez'
thumbnail: "table_wiping/table_wiping.jpg"
paperurl: 'https://arxiv.org/abs/2210.10865'
---

[[Paper](https://arxiv.org/abs/2210.10865)] 
[[Video](https://www.youtube.com/watch?v=inORKP4F3EI&feature=youtu.be)] 


<p style="text-align:center;"><img src="/images/table_wiping/crumbs.jpg" width="600"></p>

Operating in the real world requires handling high-dimensional sensory inputs and dealing with the stochasticity of the environment. In this work, we propose a framework to enable multipurpose assistive mobile robots to autonomously wipe tables to clean spills and crumbs. 

![Spills cleaning](/images/table_wiping/spills.gif)

This problem is challenging for both high-level planning and low-level control. Indeed, at a high-level, deciding how to best wipe a spill perceived by a camera requires solving a challenging planning problem with stochastic dynamics. At a
low-level, executing a wiping motion requires simultaneously maintaining contact with the table while avoiding nearby obstacles such as chairs.

Our approach combines the strengths of reinforcement learning (RL) - planning in high-dimensional observation spaces with complex stochastic dynamics, and of trajectory optimization - guaranteeing constraints satisfaction while executing whole-body trajectories. It does not require collecting a task-specific
dataset on the system and transfers zero-shot to hardware.

![approach](/images/table_wiping/approach.jpg)

Cleaning requires planning wiping actions while reasoning over uncertain multimodal latent dynamics of crumbs and spills captured via high-dimensional visual observations. To tackle this problem, we first propose a stochastic differential equation (SDE) to model crumbs and spill dynamics and absorption with a robot wiper. 

![sde](/images/table_wiping/sde.gif)

Using this model, we train a vision-based policy for planning wiping actions in simulation using reinforcement learning (RL). 

<p style="text-align:center;"><img src="/images/table_wiping/sac_network.png" width="600"></p>

To enable zero-shot sim-to-real deployment, we dovetail the RL policy with a whole-body trajectory optimization framework to compute base and arm joint trajectories that execute the desired wiping motions while guaranteeing constraints satisfaction. 

<p style="text-align:center;"><img src="/images/table_wiping/trajopt.jpg" width="800"></p>

We extensively validate our approach in simulation and on hardware.

![results](/images/table_wiping/results.jpg)


