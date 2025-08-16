---
title: "First, Learn What You Don't Know: Active Information Gathering for Driving at the Limits of Handling"
collection: publications
permalink: /publication/first_learn_what_you_dont_know
excerpt: '<br />
[Project Page](/publication/first_learn_what_you_dont_know) / 
[Paper](https://arxiv.org/abs/2411.00107) - Unstable
systems are difficult to simultaneously learn and control.'
date: 2025-08-13
# venue: 'IEEE Robotics and Automation Letters'
venue: 'RA-L'
venuetype: "journal"
paperauthors: 'A. Davydov, F. Djeumou, M. Greiff, M. Suminaka, M. Thompson, J. Subosits, T. Lew'
thumbnail: "first_learn_what_you_dont_know.jpg"
paperurl: 'https://arxiv.org/abs/2411.00107'
---

[[Paper](https://arxiv.org/abs/2411.00107)] 


Combining data-driven models that adapt online and model predictive control (MPC) has enabled effective control of nonlinear systems. However, when deployed on unstable systems, online adaptation may not be fast enough to ensure reliable simultaneous learning and control. For example, controllers on a vehicle executing highly dynamic maneuvers may push the tires to their friction limits, destabilizing the vehicle and allowing modeling errors to quickly compound and cause a loss of control.

In this work, we present a Bayesian meta-learning MPC framework. We propose an expressive vehicle dynamics model that leverages Bayesian last-layer meta-learning to enable rapid online adaptation. The model’s uncertainty estimates are used to guide informative data collection and quickly improve the model prior to deployment. Experiments on a Toyota Supra show that (i) the framework enables reliable control in dynamic drifting maneuvers, (ii) online adaptation alone may not suffice for zero-shot control of a vehicle at the edge of stability, and (iii) active data collection
helps achieve reliable performance.

<p style="text-align:center;"><img src="/images/first_learn_what_you_dont_know_big.jpg" width="500"></p>

This work leverages previous ideas on [safe active dynamics learning](/publication/seels) and demonstrates reliable vehicle control at the edge of stability. In particular, it shows that information-rich trajectories do not necessarily involve drifting, and adapting on such data aids in robust execution of challenging drifting maneuvers.

<p style="text-align:center;"><img src="/images/first_learn_what_you_dont_know_info_trajs.jpg" width="600"></p>