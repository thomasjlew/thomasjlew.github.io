---
title: "Trajectory optimization on manifolds: A theoretically-guaranteed embedded sequential convex programming approach"
collection: publications
permalink: /publication/manifold_scp
excerpt: '<br />
[Project Page](/publication/manifold_scp) / 
[Paper](https://arxiv.org/abs/1905.07654) / 
[Code](https://github.com/StanfordASL/GuSTO.jl) - 
A new SCP trajectory optimization algorithm on manifolds.'
date: 2019-05-18
# venue: 'Robotics: Science and Systems'
venue: 'RSS'
venuetype: "conference"
paperauthors: 'R. Bonalli, A. Bylard, A. Cauligi, T. Lew, M. Pavone'
thumbnail: "manifold_scp.png"
paperurl: 'https://arxiv.org/abs/1905.07654'
---

[[Paper](https://arxiv.org/abs/1905.07654)] 
[[Code](https://github.com/StanfordASL/GuSTO.jl)] 

![manifold_scp overview](/images/manifold_scp.png)

Sequential Convex Programming (SCP) has recently gained popularity as a tool for trajectory optimization due to its sound theoretical properties and practical performance. Yet, most SCP-based methods for trajectory optimization are restricted to Euclidean settings, which precludes their application to problem instances where one must reason about manifold-type constraints (that is, constraints, such as loop closure, which restrict the motion of a system to a subset of the ambient space). The aim of this paper is to fill this gap by extending SCP-based trajectory optimization methods to a manifold setting. The key insight is to leverage geometric embeddings to lift a manifold-constrained trajectory optimization problem into an equivalent problem defined over a space enjoying a Euclidean structure. This insight allows one to extend existing SCP methods to a manifold setting in a fairly natural way. In particular, we present a SCP algorithm for manifold problems with refined theoretical guarantees that resemble those derived for the Euclidean setting, and demonstrate its practical performance via numerical experiments.

### Bibtex

	@inproceedings{BonalliBylardEtAl2019,
	author = {Bonalli, R. and Bylard, A. and Cauligi, A. and Lew, T. and Pavone, M.},
	title = {Trajectory Optimization on Manifolds: {A} Theoretically-Guaranteed Embedded Sequential Convex Programming Approach},
	booktitle = {Robotics: Science and Systems},
	year = {2019},
	}
