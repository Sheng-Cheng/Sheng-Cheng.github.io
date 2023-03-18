---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

<!-- add a statement of research problems that I want to solve here. -->

Current projects
------
**L1Quad**
<iframe width="560" height="315" src="https://www.youtube.com/embed/18-2OqTRJ50" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Quadrotors are deployed to more and more applications nowadays. Yet quadrotors' flight performance is subject to various uncertainties and disturbances, e.g., ground effect, slosh payload, damaged propeller, downwash, and sudden weight change, just to name a few. In this project, we propose L1Quad: an L1 adaptive augmentation for compensating for the uncertainties and disturbances experienced by the quadrotor. We lump all the uncertainties and disturbances experienced by the quadrotor as unknown additive forces and moments which impact the quadrotor’s dynamics. An L1 adaptive augmentation is designed to estimate and compensate for these lumped uncertainties and disturbances. The video below shows the superior performance of L1Quad in various challenging scenarios without retuning the controller parameters case-by-case. All the demos were conducted on a custom-built quadrotor controlled by a Pixhawk flight controller running our customized Ardupilot firmware.  

**DiffTune**
<iframe width="560" height="315" src="https://www.youtube.com/embed/otAv1EJF7EA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The performance of a robot controller depends on the choice of its parameters, which require careful tuning. In this project, we present DiffTune, a novel, gradient-based automatic tuning framework. Our method unrolls the dynamical system and controller as a computational graph and updates the controller parameters through gradient-based optimization. The gradients are updated using sensitivity propagation (inspired by the forward-mode auto-differentiation) with real data collected from the system. 

Past projects
------
**Mobile estimation and control of a dynamical spatiotemporal process**
<iframe width="560" height="315" src="https://www.youtube.com/embed/i8Lms1cOoyI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
The long-term goal of this project is to enable multiple autonomous agents to adaptively estimate and possibly control a dynamical spatiotemporal process (e.g., harmful algal blooms or forest fires). The specific research objective is to apply tools from the theory of infinite-dimensional systems, nonlinear estimation, optimal experiment design, inverse problems, network science, uncertainty quantification, and multi-vehicle control to solve the problem of (i) estimation and control of a dynamical spatiotemporal process and (ii) task allocation for a heterogeneous group of resource-constrained agents.

**Cooperative mapping, searching, and tracking in an uncertain urban environment**
<iframe width="560" height="315" src="https://www.youtube.com/embed/9wEo0hH-psg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
In this project, we propose a cooperative mapping and search algorithm for detecting a single moving target in an urban environment that is initially unknown to a team of autonomous quadrotors equipped with noisy sensors with a limited field of view. This algorithm is being tested with real quadrotors and a simulated target at the [Fearless Flight Facility (F3)](https://aero.umd.edu/research/fearless-flight-facility-f3) of the University of Maryland. This work is in collaboration with [Dr. Artur Wolek](https://mees.charlotte.edu/directory/artur-wolek) and Heron Systems, Inc. (A Shield AI Company).
