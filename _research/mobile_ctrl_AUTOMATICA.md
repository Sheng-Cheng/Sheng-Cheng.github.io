---
title: "Optimal control of a 2D diffusion–advection process with a team of mobile actuators under jointly optimal guidance"
collection: research
type: "TBD"
permalink: /research/mbl_ctrl_automatica_2021
venue: "Automatica"
date: 2021-07-06
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
    <a href="[https://link.springer.com/article/10.1007/s10514-023-10105-9](https://www.sciencedirect.com/science/article/pii/S0005109821003873?via%3Dihub)"
       class="external-link button is-normal is-rounded is-dark">
      <span class="icon">
          <i class="fas fa-file-pdf"></i>
      </span>
      <span>Paper</span>
    </a>
  </span>
</div>

## Abstract
This paper describes an optimization framework to control a distributed parameter system (DPS) using a team of mobile actuators. The framework simultaneously seeks optimal control of the DPS and optimal guidance of the mobile actuators such that a cost function associated with both the DPS and the mobile actuators is minimized subject to the dynamics of each. The cost incurred from controlling the DPS is linear–quadratic, which is transformed into an equivalent form as a quadratic term associated with an operator-valued Riccati equation. This equivalent form reduces the problem to seeking only for guidance because the optimal control can be recovered once the optimal guidance is obtained. We establish conditions for the existence of a solution to the proposed problem. Since computing an optimal solution requires approximation, we also establish the conditions for convergence to the exact optimal solution of the approximate optimal solution. That is, when evaluating these two solutions by the original cost function, the difference becomes arbitrarily small as the approximation gets finer. Two numerical examples demonstrate the performance of the optimal control and guidance obtained from the proposed approach.

## BibTex
If you think these works are helpful to your research/application, please cite:
<pre>
@article{cheng2021optimal,
  title={Optimal control of a 2D diffusion--advection process with a team of mobile actuators under jointly optimal guidance},
  author={Cheng, Sheng and Paley, Derek A},
  journal={Automatica},
  volume={133},
  pages={109866},
  year={2021},
  publisher={Elsevier}
}
@inproceedings{cheng2020optimal,
  title={Optimal control of a 1D diffusion process with a team of mobile actuators under jointly optimal guidance},
  author={Cheng, Sheng and Paley, Derek A},
  booktitle={2020 American Control Conference (ACC)},
  pages={3449--3454},
  year={2020},
  organization={IEEE}
}
</pre>

## Acknowledgement
This research was sponsored by a seed grant from Northrop Grumman.
