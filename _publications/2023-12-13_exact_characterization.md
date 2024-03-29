---
title: "Exact Characterization of the Convex Hulls of Reachable Sets"
collection: publications
permalink: /publication/exact_characterization
excerpt: '<br />
[Project Page](/publication/exact_characterization) / 
[Paper](https://arxiv.org/abs/2303.17674v2) / 
[Code](https://github.com/StanfordASL/convex_hull_reachability) - We give a finite-dimensional characterization of the convex hulls of reachable sets of nonlinear systems (dx/dt=f(x)+w).'
date: 2023-12-13
venue: 'CDC'
venuetype: "conference"
paperauthors: 'T. Lew, R. Bonalli, M. Pavone'
thumbnail: "exact_characterization.jpg"
paperurl: 'https://arxiv.org/abs/2303.17674'
award: 'Outstanding Student Paper Award'
---

[[Paper](https://arxiv.org/abs/2303.17674v2)] 
[[Code](https://github.com/StanfordASL/convex_hull_reachability)] 


We study the convex hulls of reachable sets of nonlinear systems with bounded disturbances (dx/dt=f(x)+w). Reachable sets play a critical role in control, but [remain notoriously challenging to compute](/publication/randup). Is there additional problem structure that we can use to design faster and more accurate algorithms?

<p style="text-align:center;"><img src="/images/exact_characterization_full.jpg" width="800"></p>

In this work, we exactly characterize the convex hulls of reachable sets as the convex hulls of solutions of an ordinary differential equation from all possible initial values of the disturbances. This finite-dimensional characterization unlocks an accurate and fast estimation algorithm to over-approximate reachable sets. We present applications to neural feedback loop analysis and robust model predictive control.