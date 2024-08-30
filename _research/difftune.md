---
title: "DiffTune: Auto-Tuning through Auto-Differentiation"
collection: research
type: "TBD"
permalink: /research/DiffTune
venue: "IEEE Transactions on Robotics"
date: 2023-08
location: "City, Country"
---

<div style="text-align: center;">
  Authors: Sheng Cheng, Minkyung Kim*, Lin Song*, Chengyu Yang, Yiquan Jin, Shenlong Wang, and Naira Hovakimyan
</div>

<div style="text-align: center;">
  (* These authors contributed equally to this work.)
</div>

<div style="text-align: center;">
  University of Illinois Urbana-Champaign
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
    <a href="https://ieeexplore.ieee.org/abstract/document/10599619"
       class="external-link button is-normal is-rounded is-dark">
      <span class="icon">
          <i class="fas fa-file-pdf"></i>
      </span>
      <span>Paper</span>
    </a>
  </span>
  <span class="link-block">
    <a href="https://github.com/Sheng-Cheng/DiffTuneOpenSource"
       class="external-link button is-normal is-rounded is-dark">
      <span class="icon">
          <i class="fab fa-github"></i>
      </span>
      <span>Code</span>
    </a>
  </span>
  <span class="link-block">
    <a href="https://youtu.be/g42UxcIHUdg?si=RT13Z4kmcj1CrImu"
       class="external-link button is-normal is-rounded is-dark">
      <span class="icon">
          <i class="fab fa-youtube"></i>
      </span>
      <span>Video</span>
    </a>
  </span>
</div>

<br>
<iframe width="560" height="315" src="https://www.youtube.com/embed/g42UxcIHUdg?si=jd7aPFCTjPxSSGyv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Abstract
The performance of robots in high-level tasks depends on the quality of their lower-level controller, which requires fine-tuning. However, the intrinsically nonlinear dynamics and controllers make tuning a challenging task when it is done by hand. In this work, we present DiffTune, a novel, gradient-based automatic tuning framework. We formulate the controller tuning as a parameter optimization problem. Our method unrolls the dynamical system and controller as a computational graph (shown below) and updates the controller parameters through gradient-based optimization. The gradient is obtained using sensitivity propagation, which is the only method for gradient computation when tuning for a physical system instead of its simulated counterpart. Furthermore, we use L1 adaptive control to compensate for the uncertainties (that unavoidably exist in a physical system) such that the gradient is not biased by the unmodelled uncertainties. We validate the DiffTune on a Dubin's car and a quadrotor in challenging simulation environments. In comparison with state-of-the-art auto-tuning methods, DiffTune achieves the best performance in a more efficient manner owing to its effective usage of the first-order information of the system. Experiments on tuning a nonlinear controller for quadrotor show promising results, where DiffTune achieves 3.5x tracking error reduction on an aggressive trajectory in only 10 trials over a 12-dimensional controller. 

<div style="text-align: center;">
  <img src="/assets/figures/newDiffTuneGraph.png" alt="unrolling the system" style="width: 50%;" />
</div>

## Results of auto-tuning a nonlinear quadrotor controller
We validated DiffTune over a nonlinear geometric controller for a quadrotor trajectory tracking task. The quadrotor is commanded to track a circular trajectory with speeds of 1, 2, and 3 m/s, demonstrating gradually increased agility. The controller contains 12 parameters that govern the translational and rotational control of the quadrotor. Comparing the tracking performance at the last trial to the initial trial, the root-mean-squared error (RMSE) has achieved 1.5x, 2.5x, and 3.5x reduction on the 1, 2, and 3 m/s trajectories, respectively, which signifies the efficiency of DiffTune for performance improvement subject to nonlinear dynamics and controllers with a high-dimensional parameter space. The figures below show the tracking error reduction, evolution of the trajectory through auto-tuning trials, and the evolution of the parameters over the three trajectories.


<div style="display: flex;">
  <img src="/assets/figures/exp_RMSE_1mps-1.png" alt="Image 1" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/exp_RMSE_2mps-1.png" alt="Image 2" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/exp_RMSE_3mps-1.png" alt="Image 3" style="width: 33%;">
</div>
<div style="text-align: center;">
  Tracking RMSE of the tuning on three circular trajectories. The dashed line shows the RMSE achieved by hand-tuning.
</div>

<div style="display: flex;">
  <img src="/assets/figures/exp_trajectory_1mps-1.png" alt="Image 4" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/exp_trajectory_2mps-1.png" alt="Image 5" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/exp_trajectory_3mps-1.png" alt="Image 6" style="width: 33%;">
</div>
<div style="text-align: center;">
  Horizontal trajectories of the quadrotor during tuning on three circular trajectories with different speeds.
</div>

<div style="display: flex;">
  <img src="/assets/figures/param_1mps_new.gif" alt="gif 1" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/param_2mps_new.gif" alt="gif 2" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/param_3mps_new.gif" alt="gif 3" style="width: 33%;">
</div>
<div style="text-align: center;">
  Evolution of the parameters during the tuning on three circular trajectories with different speeds.
</div>

<br>
For more results and analysis, check the paper [here](https://ieeexplore.ieee.org/document/10599619).

## Extensions
We have extended the hyperparameter-based DiffTune to a hyperparameter-free version, DiffTune+, which optimizes the tuning process by maximizing loss reduction without the need for manually adjusting the learning rates. More details can be found in this [paper](https://proceedings.mlr.press/v211/cheng23b.html).

We have also extended target controllers of DiffTune from explicitly differentiable ones to implicitly differentiable model predictive control (MPC). The resulting architecture, DiffTune-MPC, learns an MPC's cost function in a closed-loop manner, making it compatible with scenarios where the evaluation time interval and the MPC planning horizon differ. This method has proven its efficacy in various MPC settings, including nonlinear MPCs, via analytical gradients that facilitate the auto-tuning process. More details can be found in this [paper](https://ieeexplore.ieee.org/abstract/document/10584257).


## BibTex
If you think these works are helpful to your research/application, please cite:
<pre>
@article{cheng2022difftune,
  title={DiffTune: Auto-Tuning through Auto-Differentiation},
  author={Cheng, Sheng and Kim, Minkyung and Song, Lin and Yang, Chengyu and Jin, Yiquan and Wang, Shenlong and Hovakimyan, Naira},
  journal={IEEE Transactions on Robotics},
  year={2024},
  publisher={IEEE}
}
@inproceedings{cheng2023difftunePlus,
  title={DiffTune+: Hyperparameter-Free Auto-Tuning using Auto-Differentiation},
  author={Cheng, Sheng and Song, Lin and Kim, Minkyung and Wang, Shenlong and Hovakimyan, Naira},
  booktitle={Learning for Dynamics and Control Conference},
  pages={170--183},
  year={2023},
  organization={PMLR}
}
@article{tao2024difftunempc,
  title={DiffTune-MPC: Closed-loop learning for model predictive control},
  author={Tao, Ran and Cheng, Sheng and Wang, Xiaofeng and Wang, Shenlong and Hovakimyan, Naira},
  journal={IEEE Robotics and Automation Letters},
  year={2024},
  publisher={IEEE}
}
</pre>

## Acknowledgement
This work is supported by NASA under the cooperative agreement 80NSSC20M0229,  NSF-AoF Robust Intelligence (2133656), NSF SLES (2331878), Air Force Office of Scientific Research (AFOSR) grant FA9550-21-1-0411, Amazon Research Award, and Illinois-Insper Collaborative Research Fund.
