---
layout: page
permalink: /
title: "Can a MISL Fly? Analysis and Ingredients for Mutual Information Skill Learning"
description:
nav: false
nav_order: 1
no_header: true
---

<p><center><a href="https://chongyi-zheng.github.io">Chongyi Zheng*</a>, &emsp; <a href="https://jens321.github.io">Jens Tuyls*</a>, &emsp; <a href="https://www.joannepeng.com">Joanne Peng</a>, &emsp; <a href="https://ben-eysenbach.github.io">Benjamin Eysenbach</a></center></p>
<p><center><b><a href="#">Paper</a>, &emsp; <a href="https://github.com/Princeton-RL/contrastive-successor-features">Code</a></b></center></p>

<p align="center">
<img src="assets/csf/teaser.png" width="80%" />
</p>

*__Abstract__:
Self-supervised learning has the potential of lifting several of the key challenges in reinforcement learning today, such as exploration, representation learning, and reward design. Recent work (METRA) has effectively argued that moving away from mutual information and instead optimizing a certain Wasserstein distance is important for good performance. In this paper, we argue that the benefits seen in that paper can largely be explained within the existing framework of mutual information skill learning (MISL). Our analysis suggests a new MISL method (contrastive successor features) that retains the excellent performance of METRA with fewer moving parts, and highlights connections between skill learning, contrastive representation learning, and successor features. Finally, through careful ablation studies, we provide further insight into some of the key ingredients for both our method and METRA.*


**Code**: <a href="https://github.com/Princeton-RL/contrastive-successor-features">https://github.com/Princeton-RL/contrastive-successor-features</a>

# Videos of Learned Policies

<h2>Quadruped</h2>
<hr>
<div class="row mt-12 justify-content-center">
  <div class="col-sm mt-6 mt-md-0 text-center">
    <h3>CSF</h3>
    {% include video.html path="/assets/csf/csf_quadruped_3000.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
  </div>
</div>

<div class="row mt-6 justify-content-center">
  <div class="col-sm mt-6 mt-md-0 text-center">
    <h3>METRA</h3>
    {% include video.html path="/assets/metra/metra_quadruped_3000.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
  </div>
</div>

<h2>Ant</h2>
<hr>
<div class="row mt-12 justify-content-center">
  <div class="col-sm mt-6 mt-md-0 text-center">
    <h3>CSF</h3>
    {% include video.html path="/assets/csf/csf_ant_40k.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
  </div>
</div>

<div class="row mt-6 justify-content-center">
  <div class="col-sm mt-6 mt-md-0 text-center">
    <h3>METRA</h3>
    {% include video.html path="/assets/metra/metra_ant_40k.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
  </div>
</div>

<h2>Humanoid</h2>
<hr>
<div class="row mt-12 justify-content-center">
  <div class="col-sm mt-6 mt-md-0 text-center">
    <h3>CSF</h3>
    {% include video.html path="/assets/csf/csf_humanoid_3000.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
  </div>
</div>

<div class="row mt-6 justify-content-center">
  <div class="col-sm mt-6 mt-md-0 text-center">
    <h3>METRA</h3>
    {% include video.html path="/assets/metra/metra_humanoid_3000.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
  </div>
</div>

<h2>Robobin</h2>
<hr>
<div class="row mt-12 justify-content-center">
  <div class="col-sm mt-6 mt-md-0 text-center">
    <h3>CSF</h3>
    {% include video.html path="/assets/csf/csf_robobin_3000.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
  </div>
</div>

<div class="row mt-6 justify-content-center">
  <div class="col-sm mt-6 mt-md-0 text-center">
    <h3>METRA</h3>
    {% include video.html path="/assets/metra/metra_robobin_3000.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
  </div>
</div>