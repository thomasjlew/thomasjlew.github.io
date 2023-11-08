---
title: "Risk-Averse Trajectory Optimization via Sample Average Approximation"
collection: publications
permalink: /publication/risk_averse
excerpt: '<br />
[Project Page](/publication/risk_averse) / 
[Paper](https://arxiv.org/abs/2307.03167) / 
[Code](https://github.com/StanfordASL/RiskAverseTrajOpt) - 
A sample-based approach to risk-averse trajectory optimization.'
date: 2023-10-19
venue: 'RA-L'
# venuetype: "journal"
paperauthors: 'T. Lew, R. Bonalli, M. Pavone'
thumbnail: "risk_averse.jpg"
paperurl: 'https://arxiv.org/abs/2307.03167'
---

[[Paper](https://arxiv.org/abs/2307.03167)] 
[[Code](https://github.com/StanfordASL/RiskAverseTrajOpt)]

<p style="text-align:center;"><img src="/images/risk_averse.jpg" width="600"></p>

Trajectory optimization under uncertainty underpins a wide range of applications in robotics. However, existing methods are limited in terms of reasoning about sources of epistemic and aleatoric uncertainty, space and time correlations, nonlinear dynamics, and non-convex constraints. In this work, we first introduce a continuous-time planning formulation with an average-value-at-risk constraint over the entire planning horizon. Then, we propose a sample-based approximation that unlocks an efficient and general-purpose algorithm for risk-averse trajectory optimization. We prove that the method is asymptotically optimal and derive finite-sample error bounds. Simulations demonstrate the high speed and reliability of the approach on problems with stochasticity in nonlinear dynamics, obstacle fields, interactions, and terrain parameters.
