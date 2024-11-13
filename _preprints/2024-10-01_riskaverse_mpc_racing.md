---
title: "Risk-Averse Model Predictive Control for Racing in Adverse Conditions"
collection: publications
permalink: /publication/riskaverse_mpc_racing
excerpt: '<br />
[Project Page](/publication/riskaverse_mpc_racing) / 
[Paper](https://arxiv.org/abs/2410.17183) - A risk-averse controller to reason over uncertainty.'
date: 2024-10-01
venue: 'Under Review'
# venuetype: "conference"
paperauthors: 'T. Lew, M. Greiff, F. Djeumou, M. Suminaka, M. Thompson, J. Subosits, '
thumbnail: "riskaverse_mpc_racing.jpg"
paperurl: 'https://arxiv.org/abs/2410.17183'
---

[[Paper](https://arxiv.org/abs/2410.17183)] 


Model predictive control (MPC) algorithms can be sensitive to model mismatch when used in challenging nonlinear control tasks. In particular, the performance of MPC for vehicle control at the limits of handling suffers when the underlying model overestimates the vehicle's capabilities. 

In this work, we propose a risk-averse MPC framework that explicitly accounts for uncertainty over friction limits and tire parameters. Our approach leverages a sample-based approximation of an optimal control problem with a conditional value at risk (CVaR) constraint. This sample-based formulation enables planning with a set of expressive vehicle dynamics models using different tire parameters. Moreover, this formulation enables efficient numerical resolution via sequential quadratic programming and GPU parallelization. 

Experiments on a Lexus LC 500 show that risk-averse MPC unlocks reliable performance, while a deterministic baseline that plans using a single dynamics model may lose control of the vehicle in adverse road conditions.

![riskaverse_mpc_racing_big](/images/randup/riskaverse_mpc_racing_big.jpg)

This work leverages previous ideas on [risk-averse trajectory optimization](/publication/risk_averse) to obtain an uncertainty-aware MPC scheme that reasons over
10 different dynamics models and runs at 20Hz. In particular, it shows that accounting for uncertainty enables reliable vehicle control at the edge of stability in adverse conditions.