---
title: "Learning-based warm-starting for fast sequential convex programming and trajectory optimization"
collection: publications
permalink: /publication/learning_scp
excerpt: '<br />
[Project Page](/publication/learning_scp) / 
[Paper](https://hal.archives-ouvertes.fr/hal-03467612/document) / 
[Code](https://github.com/StanfordASL/nnGuSTO) - 
We propose a learning-based strategy to warm-start trajectory optimization algorithms.'
date: 2020-03-07
# venue: 'IEEE Aerospace Conference'
venue: 'AeroConf'
venuetype: "conference"
paperauthors: 'S. Banerjee, T. Lew, R. Bonalli, A. Alfaadhel, I. Alomar, H. Shageer, M. Pavone'
thumbnail: "learning_scp.png"
paperurl: 'https://hal.archives-ouvertes.fr/hal-03467612/document'
---

[[Paper](https://hal.archives-ouvertes.fr/hal-03467612/document)] 
[[Code](https://github.com/StanfordASL/nnGuSTO)] 

![learning_scp overview](/images/learning_scp.png)

Sequential convex programming (SCP) has recently emerged as an effective tool to quickly compute locally optimal trajectories for robotic and aerospace systems alike, even when initialized with an unfeasible trajectory. In this paper, by focusing on the Guaranteed Sequential Trajectory Optimization (GuSTO) algorithm, we propose a methodology to accelerate SCP-based algorithms through warm-starting. Specifically, leveraging a dataset of expert trajectories from GuSTO, we devise a neural-network-based approach to predict a locally optimal state and control trajectory, which is used to warm-start the SCP algorithm. This approach allows one to retain all the theoretical guarantees of GuSTO while simultaneously taking advantage of the fast execution of the neural network and reducing the time and number of iterations required for GuSTO to converge. The result is a faster and theoretically guaranteed trajectory optimization algorithm.