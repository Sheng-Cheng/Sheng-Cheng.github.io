---
title: "Optimal guidance and estimation of a 2D diffusion–advection process by a team of mobile sensors"
collection: research
type: "TBD"
permalink: /research/mbl_est_automatica_2022
venue: "Automatica"
date: 2021-11-03
location: "City, Country"
---

<div style="text-align: center;">
  Authors: Sheng Cheng and Derek Paley
</div>

<div style="text-align: center;">
  University of Maryland, College Park
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
    <a href="https://www.sciencedirect.com/science/article/pii/S0005109821006415"
       class="external-link button is-normal is-rounded is-dark">
      <span class="icon">
          <i class="fas fa-file-pdf"></i>
      </span>
      <span>Paper</span>
    </a>
  </span>
</div>

## Abstract
This paper describes an optimization framework to design guidance for a possibly heterogeneous team of multiple mobile sensors to estimate a spatiotemporal process modeled by a 2D diffusion–advection process. Owing to the abstract linear system representation of the process, we apply the Kalman–Bucy filter for estimation, where the sensors provide linear outputs. We propose an optimization problem that minimizes the sum of the trace of the covariance operator of the Kalman–Bucy filter and a generic mobility cost of the mobile sensors, subject to the sensors’ motion modeled by linear dynamics. We establish the existence of a solution to this problem. Moreover, we prove convergence to the exact optimal solution of the approximate optimal solution. That is, when evaluating these two solutions using the original cost function, the difference becomes arbitrarily small as the approximation gets finer. To compute the approximate solution, we use Pontryagin’s minimum principle after approximating the infinite-dimensional terms originating from the diffusion–advection process. The approximate solution is applied in simulation to analyze how a single mobile sensor’s performance depends on two important parameters: sensor noise variance and mobility penalty. We also illustrate the application of the framework to multiple sensors, in particular the performance of a heterogeneous team of sensors.

## BibTex
If you think these works are helpful to your research/application, please cite:
<pre>
@article{cheng2022optimalEst,
  title={Optimal guidance and estimation of a 2D diffusion--advection process by a team of mobile sensors},
  author={Cheng, Sheng and Paley, Derek A},
  journal={Automatica},
  volume={137},
  pages={110112},
  year={2022},
  publisher={Elsevier}
}
@inproceedings{cheng2020optimalEst,
  title={Optimal guidance and estimation of a 1D diffusion process by a team of mobile sensors},
  author={Cheng, Sheng and Paley, Derek A},
  booktitle={2020 59th IEEE Conference on Decision and Control (CDC)},
  pages={1222--1228},
  year={2020},
  organization={IEEE}
}
</pre>

## Acknowledgement
This research was sponsored by a seed grant from Northrop Grumman.
