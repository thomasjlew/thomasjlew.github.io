---
permalink: /
title: "Thomas Lew"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


I am a research scientist at the [Toyota Research Institute](https://www.tri.global/), where I develop decision-making algorithms for autonomous systems. My research leverages tools from optimal and stochastic control, optimization, differential geometry, and machine learning, revealing insights for designing fast and reliable methods with [optimality](publication/SAA), [accuracy](publication/convex_hull_estimation), and [adaptation](publication/seels) guarantees. It was deployed on [cars](publication/riskaverse_mpc_racing), [drones](publication/cio), [spacecraft](publication/randup_l4dc) and [Mars rover](publication/exomars) testbeds, [rockets](publication/cc_rocket), and [mobile robotic manipulators](publication/table_wiping).

Previously, I received my PhD from [Stanford University](https://stanfordasl.github.io/) advised by [Marco Pavone](https://web.stanford.edu/~pavone/) and [Riccardo Bonalli](https://rbonalli.github.io/), completed research internships at [Google Brain](https://research.google/research-areas/robotics/) and [NASA JPL](https://www.jpl.nasa.gov/), and studied at [ETH Zurich](https://ethz.ch/en.html) and [EPFL](https://www.epfl.ch/en/).



<!-- News
======
10/2022: Presented our work on safe dynamics meta-learning and control at IROS 2022! Check it out here: 
-->

<!-- subtitle
------
Todo -->

# My Research
<!-- Modern autonomous systems are becoming increasingly complex and are deployed in high-uncertainty, high-stakes applications. To enable more efficient and reliable decision-making, I have been developing algorithms that explicitly account for uncertainty.--> 
Some problems I have been working on:
- *Control and optimization under uncertainty*: How can we compute [optimal trajectories](publication/SAA) for nonlinear systems that [explicitly reason over uncertainty](publication/risk_averse)? Can we find [low-dimensional structure in solutions](publication/stochastic_pmp) and leverage [GPU acceleration](publication/riskaverse_mpc_racing) to efficiently solve these problems? How can we scalably [robustify optimization-based tools via reinforcement learning](publication/diffmpc) on the GPU?
- *Forward reachability analysis*: How can we [propagate uncertainty](publication/randup_l4dc) through complex systems (potentially with neural networks in the loop) in milliseconds and use it for planning and control? What [accuracy](publication/convex_hull_estimation) can we expect? What [problem structure](publication/exact_characterization) can we exploit?
- *Reliable and efficient learning-based control*: How can a system [(meta-)learn its dynamics](publication/seels), while handling the exploration-exploitation tradeoff and always satisfying constraints? How can we [learn as fast as possible](publication/first_learn_what_you_dont_know) to enable reliable control of unstable systems?
- *Resilient navigation*: How can a drone autonomously fly [even if all its exteroceptive sensors have failed](publication/cio)?
- *Vision-based control*: How can a robot achieve precise [control from high-dimensional visual inputs](publication/table_wiping) while ensuring safe and zero-shot deployment?
<!-- a robot [autonomously and safely clean a table](publication/table_wiping)? -->

## Preprints
{% for post in site.preprints reversed %}
  {% include archive-single-paper.html %}
{% endfor %}

## Publications
{% for post in site.publications reversed %}
  {% include archive-single-paper.html %}
{% endfor %}

{% include base_path %}