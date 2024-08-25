---
title: "DiffTune: Auto-Tuning through Auto-Differentiation"
collection: test
type: "TBD"
permalink: /test/DiffTune
venue: "IEEE Transactions on Robotics"
date: 2024-08-25
location: "City, Country"
---


<div style="text-align: center;">
  Authors: Sheng Cheng, Minkyung Kim\*, Lin Song\*, Chengyu Yang, Yiquan Jin, Shenlong Wang, and Naira Hovakimyan
</div>
<div style="text-align: center;">
  (\* These authors contributed equally to this work.)
</div>
<div style="text-align: center;">
  University of Illinois Urbana-Champaign
</div>


## Demo
<iframe width="560" height="315" src="https://www.youtube.com/embed/g42UxcIHUdg?si=jd7aPFCTjPxSSGyv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Abstract
The performance of robots in high-level tasks depends on the quality of their lower-level controller, which requires fine-tuning. However, the intrinsically nonlinear dynamics and controllers make tuning a challenging task when it is done by hand. In this work, we present DiffTune, a novel, gradient-based automatic tuning framework. We formulate the controller tuning as a parameter optimization problem. Our method unrolls the dynamical system and controller as a computational graph and updates the controller parameters through gradient-based optimization. The gradient is obtained using sensitivity propagation, which is the only method for gradient computation when tuning for a physical system instead of its simulated counterpart. Furthermore, we use L1 adaptive control to compensate for the uncertainties (that unavoidably exist in a physical system) such that the gradient is not biased by the unmodelled uncertainties. We validate the DiffTune on a Dubin's car and a quadrotor in challenging simulation environments. In comparison with state-of-the-art auto-tuning methods, DiffTune achieves the best performance in a more efficient manner owing to its effective usage of the first-order information of the system. Experiments on tuning a nonlinear controller for quadrotor show promising results, where DiffTune achieves 3.5x tracking error reduction on an aggressive trajectory in only 10 trials over a 12-dimensional controller. 

## Overview
Some descriptions of the framework. Put the figure to side rather than take a huge space in the middle
![Description of the image](/assets/figures/DiffTune_comp_graph.png)

## Results
Gif showing param evolution (from slides) and tracking error plots (in paper)


<div style="display: flex;">
  <img src="/assets/figures/exp_RMSE_1mps-1.png" alt="Image 1" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/exp_RMSE_2mps-1.png" alt="Image 2" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/exp_RMSE_3mps-1.png" alt="Image 3" style="width: 33%;">
</div>

Need to have the caption here

<div style="display: flex;">
  <img src="/assets/figures/exp_trajectory_1mps-1.png" alt="Image 1" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/exp_trajectory_2mps-1.png" alt="Image 2" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/exp_trajectory_3mps-1.png" alt="Image 3" style="width: 33%;">
</div>

Need to have the caption here

<div style="display: flex;">
  <img src="/assets/figures/param_1mps_new.gif" alt="Image 1" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/param_2mps_new.gif" alt="Image 2" style="width: 33%; margin-right: 5px;">
  <img src="/assets/figures/param_3mps_new.gif" alt="Image 3" style="width: 33%;">
</div>
Need to have the caption here

For more results, check the paper

Extensions

## Bib
```
@article{cheng2022difftune,
  title={DiffTune: Auto-Tuning through Auto-Differentiation},
  author={Cheng, Sheng and Kim, Minkyung and Song, Lin and Yang, Chengyu and Jin, Yiquan and Wang, Shenlong and Hovakimyan, Naira},
  journal={accepted for publication by IEEE Transactions on Robotics, arXiv preprint arXiv:2209.10021},
  year={2024}
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
  title={{DiffTune-MPC}: Closed-loop learning for model predictive control},
  author={Tao, Ran and Cheng, Sheng and Wang, Xiaofeng and Wang, Shenlong and Hovakimyan, Naira},
  journal={IEEE Robotics and Automation Letters},
  year={2024},
  publisher={IEEE}
}
```

## Acknowledgement
This work is supported by NASA under the cooperative agreement 80NSSC20M0229,  NSF-AoF Robust Intelligence (2133656), NSF SLES (2331878), Air Force Office of Scientific Research (AFOSR) grant FA9550-21-1-0411, Amazon Research Award, and Illinois-Insper Collaborative Research Fund.
