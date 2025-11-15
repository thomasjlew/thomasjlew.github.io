---
permalink: /
title: "Thomas Lew"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


I am a research scientist at the [Toyota Research Institute](https://www.tri.global/), where I develop decision-making algorithms for autonomous systems. My research leverages tools from optimal and stochastic control, optimization, differential geometry, and machine learning to design fast and reliable methods with [optimality](publication/SAA), [accuracy](publication/convex_hull_estimation), and [adaptation](publication/seels) guarantees. These algorithms have been deployed on [cars](publication/riskaverse_mpc_racing), [drones](publication/cio), [spacecraft](publication/randup_l4dc) and [Mars rover](publication/exomars) testbeds, [rockets](publication/cc_rocket), and [mobile manipulators](publication/table_wiping).

Previously, I received my PhD from [Stanford University](https://stanfordasl.github.io/) advised by [Marco Pavone](https://web.stanford.edu/~pavone/) and [Riccardo Bonalli](https://rbonalli.github.io/), completed research internships at [Google Brain](https://research.google/research-areas/robotics/) and [NASA JPL](https://www.jpl.nasa.gov/), and studied at [ETH Zurich](https://ethz.ch/en.html) and [EPFL](https://www.epfl.ch/en/).



# My Research
My work develops reliable and scalable decision-making algorithms for autonomous systems. Current directions include:
- *Uncertainty-aware control*: Methods that explicitly reason about uncertainty with [optimality guarantees](publication/SAA) and [robust performance](publication/riskaverse_mpc_racing), and theory that reveals [low-dimensional solution structure](publication/stochastic_pmp) in stochastic control to unlock faster algorithms.
- *GPU-accelerated optimization*: Differentiable solvers tailored to GPU parallelism, enabling fast [uncertainty-aware MPC](publication/riskaverse_mpc_racing) and scalable integration into [reinforcement learning](publication/diffmpc).
- *Reachability & uncertainty propagation*: Real-time tools for [propagating uncertainty](publication/randup_l4dc) through nonlinear and neural network  models, with [provable accuracy](publication/convex_hull_estimation) and using [low-dimensional characterizations](publication/exact_characterization) of reachable sets.
- *Reliable learning-based control*: Safe and data-efficient algorithms to [learn dynamics](publication/seels), balance exploration and exploitation, and achieve  reliable [learning-based control of unstable systems](publication/first_learn_what_you_dont_know).
- *Embodied autonomy*: Algorithms enabling robust performance in challenging settings, such as [perception-degraded flight](publication/cio) and [vision-based manipulation tasks](publication/table_wiping).


## Preprints
{% for post in site.preprints reversed %}
  {% include archive-single-paper.html %}
{% endfor %}

## Publications
{% for post in site.publications reversed %}
  {% include archive-single-paper.html %}
{% endfor %}

{% include base_path %}