---
permalink: /
title: "Thomas Lew"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a PhD student at [Stanford](https://stanfordasl.github.io/) advised by [Prof. Marco Pavone](https://web.stanford.edu/~pavone/). I previously studied at [ETH Zurich](https://ethz.ch/en.html) and [EPFL](https://www.epfl.ch/en/), and completed research internships at [Google Brain Robotics](https://research.google/research-areas/robotics/) and [NASA JPL](https://www.jpl.nasa.gov/).

<!-- I develop algorithms for more reliable robotic autonomy using tools from optimal control, stochastic calculus, differential geometry, and deep learning. My research is grounded in theory, revealing insights for designing faster methods with [optimality](publication/SAA), [accuracy](publication/randup_l4dc), and [adaptation](publication/seels) guarantees. It was deployed on [drones](publication/cio), [spacecraft](publication/randup_l4dc) and [Mars rover](publication/exomars) testbeds, [rockets](publication/cc_rocket), and [mobile manipulators](publication/table_wiping). -->

<!-- I develop algorithms for the reliable control of autonomous systems.  -->
I develop decision-making algorithms for autonomous systems. My work leverages tools from optimal control, stochastic calculus, differential geometry, and deep learning, revealing insights for designing fast and reliable methods with [optimality](publication/SAA), [accuracy](publication/randup_l4dc), and [adaptation](publication/seels) guarantees. It was deployed on [drones](publication/cio), [spacecraft](publication/randup_l4dc) and [Mars rover](publication/exomars) testbeds, [rockets](publication/cc_rocket), and [mobile manipulators](publication/table_wiping).


<!-- News
======
10/2022: Presented our work on safe dynamics meta-learning and control at IROS 2022! Check it out here: 
-->

<!-- subtitle
------
Todo -->

# My Research
Some problems I have been working on:
- How can we compute [optimal trajectories](publication/SAA) for uncertain nonlinear dynamical systems? 
- How can we [propagate uncertainty](publication/randup_l4dc) through complex systems (potentially with neural networks in the loop) in milliseconds, and use it for planning and control?
- How can a system [safely (meta-)learn its dynamics](publication/seels)? How can we handle the exploration-exploitation tradeoff while satisfying constraints?
- How can a drone [autonomously fly even if all its exteroceptive sensors have failed](publication/cio)?
- How can we achieve precise [control from high-dimensional visual inputs](publication/table_wiping) while ensuring safe deployment in stochastic environments?
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