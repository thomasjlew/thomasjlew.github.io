---
title: "Rough Stochastic Pontryagin Maximum Principle and an Indirect Shooting Method"
collection: publications
permalink: /publication/stochastic_pmp
excerpt: '<br />
[Project Page](/publication/stochastic_pmp) / 
[Paper](https://arxiv.org/abs/2502.06726) / 
[Code](https://github.com/ToyotaResearchInstitute/rspmp) / 
[Summary](https://github.com/thomasjlew/thomasjlew.github.io/tree/master/files/RSPMP_trajectory_optimization.pdf) - We derive new optimality conditions and an indirect method for stochastic optimal control.'
date: 2025-11-07
venue: 'SICON'
# venuetype: "journal"
paperauthors: 'T. Lew'
thumbnail: "stochastic_pmp.png"
paperurl: 'https://arxiv.org/abs/2502.06726'
---

[[Paper](https://arxiv.org/abs/2502.06726)] 
[[Summary](https://github.com/thomasjlew/thomasjlew.github.io/tree/master/files/RSPMP_trajectory_optimization.pdf)] 
[[Code](https://github.com/ToyotaResearchInstitute/rspmp)]


We study necessary optimality conditions for stochastic optimal control, which has found numerous applications such as in finance, aerospace, and robotics. Existing results are often expressed as a stochastic Pontryagin Maximum Principle (PMP) involving forward-backward stochastic differential equations (FBSDEs), and have been key to understand the solutions to these problems. For problems with linear dynamics and linear-quadratic costs for example, the PMP leads to tractable solutions characterized by stochastic Riccati equations. However, the complexity of existing PMPs with FBSDEs has hindered applications of these results to solve nonlinear stochastic optimal control problems. In deterministic optimal control on the other hand, the PMP provides low-dimensional characterizations of optimal solutions and informs the design of efficient indirect shooting methods for nonlinear optimal control. Can we derive a simpler PMP for the stochastic setting that also guides the design of efficient algorithms?

In this work, we derive a new PMP for open-loop stochastic optimal control for systems modeled by rough differential equations (RDEs) driven by Gaussian rough paths. This PMP applies to systems following SDEs driven by Brownian motion, yet it does not rely on FBSDEs and involves the same Hamiltonian as the deterministic PMP. The adjoint equation is interpreted pathwise (like in the deterministic setting) via rough path theory, simplifying the formulation of the PMP.

As an application, we propose the first indirect shooting method for nonlinear stochastic optimal control and show that it converges 10x faster than a [direct method](/publication/SAA) on a regulation task.

![stochastic_pmp_2](/images/stochastic_pmp_2.png)

Shown above is the solution returned by the indirect shooting method with the (stochastic) state trajectories (left), the control trajectory (middle), and the adjoint vector trajectories (right) satisfying the PMP. The state and control trajectories converge to zero over time (in average for the state trajectories). The adjoint vector trajectories start from different initial conditions and are all zero at the final time to satisfy the transversality condition of the PMP.