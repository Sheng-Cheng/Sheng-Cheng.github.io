---
title: "Cooperative estimation and control of a diffusion-based spatiotemporal process using mobile sensors and actuators"
collection: research
type: "TBD"
excerpt: ""
permalink: /research/auro_2023
venue: " Autonomous Robots"
date: 2022-01-09
location: "City, Country"
---

<div style="text-align: center;">
  Authors: Sheng Cheng<sup>1</sup> and Derek Paley<sup>2</sup>
</div>

<div style="text-align: center;">
  <sup>1</sup>University of Illinois Urbana-Champaign<br>
  <sup>2</sup>University of Maryland, College Park
</div>

<!-- Add custom CSS for centering the buttons -->
<style>
  .centered-buttons {
    text-align: center; /* Center-align the content */
    margin-top: 20px;   /* Add top margin for spacing */
  }

  .link-block {
    margin: 0 10px; /* Add spacing between buttons */
    display: inline-block; /* Ensure buttons are displayed inline */
  }
</style>

<!-- HTML for the centered buttons -->
<div class="centered-buttons">
  <span class="link-block">
    <a href="https://link.springer.com/article/10.1007/s10514-023-10105-9"
       class="external-link button is-normal is-rounded is-dark">
      <span class="icon">
          <i class="fas fa-file-pdf"></i>
      </span>
      <span>Paper</span>
    </a>
  </span>
  <span class="link-block">
    <a href="https://www.youtube.com/watch?v=i8Lms1cOoyI"
       class="external-link button is-normal is-rounded is-dark">
      <span class="icon">
          <i class="fab fa-youtube"></i>
      </span>
      <span>Video</span>
    </a>
  </span>
</div>

<br>
<iframe width="560" height="315" src="https://www.youtube.com/embed/i8Lms1cOoyI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Abstract
Monitoring and controlling a large-scale spatiotemporal process can be costly and dangerous for human operators, which can delegate the task to mobile robots for improved efficiency at a lower cost. The complex evolution of the spatiotemporal process and limited onboard resources of the robots motivate a holistic design of the robots’ actions to complete the tasks efficiently. This paper describes a cooperative framework for estimating and controlling a spatiotemporal process using a team of mobile robots that have limited onboard resources. We model the spatiotemporal process as a 2D diffusion equation that can characterize the intrinsic dynamics of the process with a partial differential equation (PDE). Measurement and actuation of the diffusion process are performed by mobile robots carrying sensors and actuators. The core of the framework is a nonlinear optimization problem, that simultaneously seeks the actuation and guidance of the robots to control the spatiotemporal process subject to the PDE dynamics. The limited onboard resources are formulated as inequality constraints on the actuation and speed of the robots. Extensive numerical studies analyze and evaluate the proposed framework using nondimensionalization and compare the optimal strategy to baseline strategies. The framework is demonstrated on an outdoor multi-quadrotor testbed using hardware-in-the-loop simulations.

## BibTex
If you think these works are helpful to your research/application, please cite:
<pre>
@article{cheng2023cooperative,
  title={Cooperative estimation and control of a diffusion-based spatiotemporal process using mobile sensors and actuators},
  author={Cheng, Sheng and Paley, Derek A},
  journal={Autonomous Robots},
  volume={47},
  number={6},
  pages={715--731},
  year={2023},
  publisher={Springer}
}
</pre>

## Acknowledgement
This research is supported by a seed grant from Northrop Grumman.
