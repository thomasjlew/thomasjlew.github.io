---
title: "Estimating the convex hull of the image of a set with smooth boundary: error bounds and applications"
collection: publications
permalink: /publication/convex_hull_estimation
excerpt: '<br />
[Project Page](/publication/convex_hull_estimation) / 
[Paper](https://arxiv.org/abs/2302.13970) / 
[Code](https://github.com/StanfordASL/convex-hull-estimation) - 
We study the problem of estimating the convex hull of the image of a compact set with smooth boundary.'
date: 2023-02-27
venue: 'Under Review'
# venuetype: "journal"
paperauthors: 'T. Lew, R. Bonalli, L. Janson, M. Pavone'
thumbnail: "convex_hull_estimation.png"
paperurl: 'https://arxiv.org/abs/2302.13970'
---

[[Paper](https://arxiv.org/abs/2302.13970)] 
[[Code](https://github.com/StanfordASL/convex-hull-estimation)]

<p style="text-align:center;"><img src="/images/convex_hull_estimation_full.png" width="300"></p>

### Abtract

We study the problem of estimating the convex hull of the image f(X) of a compact set X with smooth boundary through a smooth function f. Assuming that the function is a diffeomorphism or a submersion, we derive new bounds on the Hausdorff distance between the convex hull of f(X) and the convex hull of the images f(xi) of M samples xi on the boundary of X. When applied to the problem of geometric inference from random samples, our results give tighter and more general error bounds than the state of the art. We present applications to the problems of robust optimization, of reachability analysis of dynamical systems, and of robust trajectory optimization under bounded uncertainty. 

### Connection to forward reachability analysis

The results in this paper better explain the accuracy of the sampling-based reachability analysis algorithm described in [this project](/publication/randup). In particular, we derive new error bounds that are significantly tighter than the bounds from this [previous project](/publication/randup_l4dc). The missing piece was accounting for the smoothness of the boundaries of the sets of interest, which can be made rigorous using differential geometry and allows deriving tight error bounds for convex hull estimators.
