---
title: "Robust-RRT: Probabilistically-Complete Motion Planning for Uncertain Nonlinear Systems"
collection: publications
permalink: /publication/robustrrt
excerpt: '<br />
[Project Page](/publication/robustrrt) / 
[Paper](https://arxiv.org/abs/2205.07728) / 
[Code](https://github.com/StanfordASL/randUP_RRT.git) - 
A robust sampling-based motion planning algorithm.'
date: 2022-09-25
# venue: 'International Symposium on Robotics Research'
venue: 'ISRR'
venuetype: "conference"
paperauthors: 'A. Wu, T. Lew, K. Solovey, E. Schmerling, M. Pavone'
thumbnail: "robustrrt.png"
paperurl: 'https://arxiv.org/abs/2205.07728'
---

[[Paper](https://arxiv.org/abs/2205.07728)] 
[[Code](https://github.com/StanfordASL/randUP_RRT.git)] 

We present a sampling-based algorithm for computing motion plans that explicitly account for uncertainty: it returns robust motion plans that satisfy system dynamics, respect all constraints, avoid obstacles, and reach the goal for all possible uncertainty realizations belonging to a bounded set. Importantly, we prove the probabilistic completeness of the algorithm: it will eventually find a valid solution if there exists one. 


Our method applies to a broad class of complex systems and works with black-box simulators. 

<img src="/images/robustrrt/pusher.png" width="160" height="10"/>
<img src="/images/robustrrt/pusher_traj.gif" width="600" height="25"/>

It can handle both epistemic (such as uncertain model parameters) and aleatoric (such as external disturbances due to wind) sources of uncertainty.

<img src="/images/robustrrt/drone1.jpg" width="350" height="15"/>
<img src="/images/robustrrt/drone2.jpg" width="350" height="15"/>

Standard RRT consists of constructing a tree of states. In this work, we extend this concept by constructing a *tree of reachable sets*, where each set corresponds to all states that can be reached for all possible uncertain parameters and disturbances). Using a new [sampling-based algorithm](randup_l4dc), these forward reachable sets can be efficiently computed for general classes of systems.

![robustrrt overview](/images/robustrrt.png)

We also verify our method on a jumping robotic system with uncertain guard surfaces.

<img src="/images/robustrrt/jumper.png" width="250" height="30"/>
<img src="/images/robustrrt/jumper_traj.gif" width="500" height="25"/>

<!-- ### Abstract

Robust motion planning entails computing a global motion plan that is safe under all possible uncertainty realizations, be it in the system dynamics, the robot's initial position, or with respect to external disturbances. Current approaches for robust motion planning either lack theoretical guarantees, or make restrictive assumptions on the system dynamics and uncertainty distributions. In this paper, we address these limitations by proposing the robust rapidly-exploring random-tree (Robust-RRT) algorithm, which integrates forward reachability analysis directly into sampling-based control trajectory synthesis. We prove that Robust-RRT is probabilistically complete (PC) for nonlinear Lipschitz continuous dynamical systems with bounded uncertainty. In other words, Robust-RRT eventually finds a robust motion plan that is feasible under all possible uncertainty realizations assuming such a plan exists. Our analysis applies even to unstable systems that admit only short-horizon feasible plans; this is because we explicitly consider the time evolution of reachable sets along control trajectories. Thanks to the explicit consideration of time dependency in our analysis, PC applies to unstabilizable systems. To the best of our knowledge, this is the most general PC proof for robust sampling-based motion planning, in terms of the types of uncertainties and dynamical systems it can handle. Considering that an exact computation of reachable sets can be computationally expensive for some dynamical systems, we incorporate sampling-based reachability analysis into Robust-RRT and demonstrate our robust planner on nonlinear, underactuated, and hybrid systems. -->

### Bibtex

	@inproceedings{WuLewEtAl2022,
		author = {Wu, A. and Lew, T. and Solovey, K. and Schmerling, E. and Pavone, M.},
		booktitle = {International Symposium on Robotics Research},
		title = {Robust-RRT: Probabilistically-Complete Motion Planning for Uncertain Nonlinear Systems},
		year = {2022},
	}
