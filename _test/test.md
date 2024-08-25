---
title: "DiffTune website test"
collection: test
type: "TBD"
permalink: /test/DiffTune
venue: "TBD"
date: 2024-08-25
location: "City, Country"
---

DiffTune: Auto-Tuning through Auto-Differentiation

Sheng Cheng, Minkyung Kim$^*$, Lin Song$^*$, Chengyu Yang, Yiquan Jin, Shenlong Wang, and Naira Hovakimyan

University of Illinois Urbana-Champaign

![Description of the image](/assets/figures/DiffTune_exp_longexposure.png)


The performance of robots in high-level tasks depends on the quality of their lower-level controller, which requires fine-tuning. However, the intrinsically nonlinear dynamics and controllers make tuning a challenging task when it is done by hand. In this work, we present DiffTune, a novel, gradient-based automatic tuning framework. We formulate the controller tuning as a parameter optimization problem. Our method unrolls the dynamical system and controller as a computational graph 
and updates the controller parameters through gradient-based optimization. The gradient is obtained using sensitivity propagation, which is the only method for gradient computation when tuning for a physical system instead of its simulated counterpart. Furthermore, we use L1 adaptive control to compensate for the uncertainties (that unavoidably exist in a physical system) such that the gradient is not biased by the unmodelled uncertainties. We validate the DiffTune on a Dubin's car and a quadrotor in challenging simulation environments. In comparison with state-of-the-art auto-tuning methods, DiffTune achieves the best performance in a more efficient manner owing to its effective usage of the first-order information of the system. Experiments on tuning a nonlinear controller for quadrotor show promising results, where DiffTune achieves 3.5x tracking error reduction on an aggressive trajectory in only 10 trials over a 12-dimensional controller. 

Overview

![Description of the image](/assets/figures/DiffTune_comp_graph.png)

Results

<iframe width="560" height="315" src="https://www.youtube.com/embed/g42UxcIHUdg?si=jd7aPFCTjPxSSGyv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Gif showing param evolution (from slides) and tracking error plots (in paper)

<p float="left">
  <img src="/assets/figures/exp_RMSE_1mps-1.png" width="33%" />
  <img src="/assets/figures/exp_RMSE_2mps-1.png" width="33%" />
  <img src="/assets/figures/exp_RMSE_3mps-1.png" width="33%" />
</p>

<div style="display: flex;">
  <img src="/assets/figures/exp_trajectory_1mps-1.png" alt="Image 1" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/exp_trajectory_1mps-1.png" alt="Image 2" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/exp_trajectory_1mps-1.png" alt="Image 3" style="width: 33%;">
</div>

<p float="left">
  <img src="/assets/figures/param_1mps_new.gif" width="33%" />
  <img src="/assets/figures/param_2mps_new.gif" width="33%" />
  <img src="/assets/figures/param_3mps_new.gif" width="33%" />
</p>

Extensions

Bib

Ack

