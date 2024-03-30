---
title: "Control Barrier Functions for Cyber-Physical Systems and Applications to NMPC"
collection: publications
permalink: /publication/cbfs_delays
excerpt: '<br />
[Project Page](/publication/cbfs_delays) / 
[Paper](https://arxiv.org/abs/2104.14250) - 
We propose a CBF formulation that accounts for delays.'
date: 2021-04-29
# venue: 'IEEE Robotics and Automation Letters'
venue: 'RA-L'
venuetype: "journal"
paperauthors: 'J. Schilliger, T. Lew, S. Richards, S. Hänggi, M. Pavone, C. Onder'
thumbnail: "cbfs_delays.png"
paperurl: 'https://arxiv.org/abs/2104.14250'
---

[[Paper](https://arxiv.org/abs/2104.14250)] 

Tractable safety-ensuring algorithms for cyber-physical systems are important in critical applications. Approaches based on Control Barrier Functions assume continuous enforcement, which is not possible in an online fashion. This paper presents two tractable algorithms to ensure forward invariance of discrete-time controlled cyber-physical systems. Both approaches are based on Control Barrier Functions to provide strict mathematical safety guarantees. The first algorithm exploits Lipschitz continuity and formulates the safety condition as a robust program which is subsequently relaxed to a set of affine conditions. The second algorithm is inspired by tube-NMPC and uses an affine Control Barrier Function formulation in conjunction with an auxiliary controller to guarantee safety of the system. We combine an approximate NMPC controller with the second algorithm to guarantee strict safety despite approximated constraints and show its effectiveness experimentally on a mini-Segway.