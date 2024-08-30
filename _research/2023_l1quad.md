---
title: "L1Quad: L1 Adaptive Augmentation of Geometric Control for Agile Quadrotors with Performance Guarantees"
collection: research
type: "TBD"
permalink: /research/l1quad
venue: "under review"
date: 2023-02-01
location: "City, Country"
---

<div style="text-align: center;">
  Authors: Zhuohuan Wu*, Sheng Cheng*, Pan Zhao, Aditya Gahlawat, Kasey A. Ackerman, Arun Lakshmanan, Chengyu Yang, Jiahao Yu and Naira Hovakimyan
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
    <a href="https://arxiv.org/abs/2302.07208"
       class="external-link button is-normal is-rounded is-dark">
      <span class="icon">
          <i class="fas fa-file-pdf"></i>
      </span>
      <span>Paper</span>
    </a>
  </span>
  <span class="link-block">
    <a href="https://youtu.be/18-2OqTRJ50"
       class="external-link button is-normal is-rounded is-dark">
      <span class="icon">
          <i class="fab fa-youtube"></i>
      </span>
      <span>Video</span>
    </a>
  </span>
  <span class="link-block">
    <a href="https://github.com/sigma-pi/L1Quad"
       class="external-link button is-normal is-rounded is-dark">
      <span class="icon">
          <i class="fab fa-github"></i>
      </span>
      <span>Code (Ardupilot)</span>
    </a>
  </span>
  <span class="link-block">
    <a href="https://github.com/cfc-ray/L1-Crazyflie"
       class="external-link button is-normal is-rounded is-dark">
      <span class="icon">
          <i class="fab fa-github"></i>
      </span>
      <span>Code (Crazyflie)</span>
    </a>
  </span>
  <span class="link-block">
    <a href="https://github.com/HovakimyanResearch/L1-Mambo"
       class="external-link button is-normal is-rounded is-dark">
      <span class="icon">
          <i class="fab fa-github"></i>
      </span>
      <span>Code (Parrot Mambo)</span>
    </a>
  </span>
</div>

<br>
<iframe width="560" height="315" src="https://www.youtube.com/embed/18-2OqTRJ50" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Abstract
Quadrotors are deployed to more and more applications nowadays. Yet quadrotors' flight performance is subject to various uncertainties and disturbances, e.g., ground effect, slosh payload, damaged propeller, downwash, and sudden weight change, just to name a few. In this project, we propose L1Quad: an L1 adaptive augmentation for compensating for the uncertainties and disturbances experienced by the quadrotor. We lump all the uncertainties and disturbances experienced by the quadrotor as unknown additive forces and moments which impact the quadrotor’s dynamics. An L1 adaptive augmentation is designed to estimate and compensate for these lumped uncertainties and disturbances. The video below shows the superior performance of L1Quad in various challenging scenarios without retuning the controller parameters case-by-case. All the demos were conducted on a custom-built quadrotor controlled by a Pixhawk flight controller running our customized Ardupilot firmware.  

## BibTex
If you think these works are helpful to your research/application, please cite:
<pre>
@article{wu2023L1quad,
  title={$\mathcal{L}_1$Quad: $\mathcal{L}_1$ Adaptive Augmentation of Geometric Control for Agile Quadrotors with Performance Guarantees},
  author={Wu, Zhuohuan and Cheng, Sheng and Zhao, Pan and Gahlawat, Aditya and Ackerman, Kasey A and Lakshmanan, Arun and Yang, Chengyu and Yu, Jiahao and Hovakimyan, Naira},
  journal={arXiv preprint arXiv:2302.07208},
  year={2023}
}
@inproceedings{wu20221,
  title={L1 adaptive augmentation for geometric tracking control of quadrotors},
  author={Wu, Zhuohuan and Cheng, Sheng and Ackerman, Kasey A and Gahlawat, Aditya and Lakshmanan, Arun and Zhao, Pan and Hovakimyan, Naira},
  booktitle={2022 International Conference on Robotics and Automation (ICRA)},
  pages={1329--1336},
  year={2022},
  organization={IEEE}
}
</pre>

## Acknowledgement
This work is supported by National Aeronautics and Space Administration (NASA) grant 80NSSC22M0070, National Science Foundation (NSF) under the RI grant 2133656 and Air Force Office of Scientific Research.
