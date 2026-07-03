---
title: "Boundary Sampling to Learn Predictive Safety Filters via Pontryagin's Maximum Principle"
collection: publications
permalink: /publication/pmpsampling
excerpt: '<br />
[Project Page](/publication/pmpsampling) / 
[Paper](https://arxiv.org/abs/2604.13325) - Data Generation for Learned HJB Safety Filtering.'
date: 2026-07-02
venue: 'Under Review'
# venuetype: "journal"
paperauthors: 'J. Dallas, T. Lew, J. Talbot, J. DeCastro, S. Bansal, J. Subosits'
thumbnail: "pmpsampling/pmpsampling_small.jpg"
paperurl: 'https://arxiv.org/abs/2604.13325'
---

[[Paper](https://arxiv.org/abs/2604.13325)]

Learned safety filters, e.g., using deep learning to approximate the solutions to HJB, are only as good as the data that they are trained on. While such learning-based tools scale to high-dimensional systems, their performance depends on informative data that includes states likely to lead to constraint violation, which can be difficult to efficiently sample in complex, high-dimensional systems.

In this work, we leverage [previous results](/publication/convex_hulls_reachable_sets) using the Pontryagin Maximum Principle to characterize trajectories that barely avoid constraints violations, to guide data collection for learned Hamilton-Jacobi Reachability and concentrate learning efforts near safety-critical states to improve efficiency.

![pmpsampling](/images/pmpsampling.jpg)

The learned Control Barrier Value Function is then used directly for safety filtering. Simulations and experimental validation on a shared-control automotive racing application demonstrate PMP sampling improves learning efficiency, yielding faster convergence, reduced failure rates, and improved safe set reconstruction.

<p style="text-align:center;"><img src="/images/randup/pmpsampling_platform.png" width="300"></p>