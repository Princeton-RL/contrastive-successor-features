---
layout: page
permalink: /
title: "C-Learning: Learning to Achieve Goals via Recursive Classification"
description:
nav: false
nav_order: 1
---

<p><center><a href="https://ben-eysenbach.github.io/">Benjamin Eysenbach</a>, &emsp; <a href="https://tianjunz.github.io/">Tianjun Zhang</a>, &emsp; <a href="https://www.cs.cmu.edu/~rsalakhu/">Ruslan Salakhutdinov</a>, &emsp; <a href="https://people.eecs.berkeley.edu/~svlevine/">Sergey Levine</a></center></p>
<p><center><b><a href="https://arxiv.org/abs/2206.07568">Paper</a>, &emsp; <a href="https://github.com/google-research/google-research/tree/master/contrastive_rl">Code</a>, &emsp;  <a href="https://youtu.be/5_eGcprfw60">Video</a></b></center></p>

*__tldr__:
We reframe goal-conditioned RL as the problem of predicting and controlling the future state distribution of an autonomous agent. We solve this problem indirectly by training a classifier to predict whether an observation comes from the future. Importantly, an off-policy variant of our algorithm allows us to predict the future state distribution of a new policy, without collecting new experience. While conceptually similar to Q-learning, our approach provides a theoretical justification for goal-relabeling methods employed in prior work and suggests how the goal-sampling ratio can be optimally chosen. Empirically our method outperforms these prior methods.*

**Code**: https://github.com/google-research/google-research/tree/master/c_learning

# Videos of Learned Policies
Below, we visualize examples of the behavoir learned by our method. We emphasize that our method does not use any reward shaping or hand-crafted distance functions. Note that the robot has learned to retry if it initially fails to solve the task, and has learned to finely adjust the position of the objects if its initial attempt slightly missed the goal.

### Sawyer Pushing
In this task, the robot is supposed to move the red puck to the goal, which is indicated by the green circle.


<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
    {% include video.html path="../assets/c_learning/sawyer_push_1.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
    {% include video.html path="../assets/c_learning/sawyer_push_2.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true  %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
    {% include video.html path="../assets/c_learning/sawyer_push_3.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_push_4.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_push_5.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_push_6.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<!-- <div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_push_7.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_push_8.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_push_9.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div> -->
<!-- {% include video.html path="../assets/c_learning/sawyer_push_10.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true%} -->


### Sawyer Pick
In this task, the robot is supposed to pick up the puck and lift it to the green circle.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_lift_1.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_lift_2.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_lift_3.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_lift_4.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_lift_5.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_lift_6.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>


### Sawyer Window
In this task, the robot is supposed to slide the window so that the handle is aligned with the green circle.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_window_1.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_window_2.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_window_3.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_window_4.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_window_5.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_window_6.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>

### Sawyer Drawer
In this task, the robot is supposed to pull or push the drawer so the handle is aligned with the green circle.


<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_drawer_1.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_drawer_2.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_drawer_3.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_drawer_4.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_drawer_5.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_drawer_6.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>

### Sawyer Faucet
In this task, the robot is supposed to turn the faucet to the handle is aligned with the (tiny) green circle.


<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_faucet_1.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_faucet_2.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_faucet_3.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_faucet_4.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_faucet_5.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_faucet_6.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>

<!-- ![7](../assets/c_learning//sawyer_faucet_7.mp4 width="100%") ![8](../assets/c_learning//sawyer_faucet_8.mp4 width="100%") -->

### Sawyer Push Two
In this task, the robot is supposed to push two pucks to their respective goals (green goal for green puck, red goal for red puck).


<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_push_two_1.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_push_two_2.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_push_two_3.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_push_two_4.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_push_two_5.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="../assets/c_learning/sawyer_push_two_6.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>


# Predictions of the Future State Distribution
Our method predicts where an agent is likely to be in the time-discounted future. Below, we give our model an observation (top) and action (not shown) and it predicts a distribution over future states (bottom). As expected, the model predicts more distant states when we increase the discount factor $$\gamma$$.

{% include figure.html path="../assets/c_learning/Ant-v2_gamma_0.50.gif" class="img-fluid rounded z-depth-1" caption="Ant-v2, $$\gamma = 0.5$$" %}
{% include figure.html path="../assets/c_learning/Ant-v2_gamma_0.90.gif" class="img-fluid rounded z-depth-1" caption="Ant-v2, $$\gamma = 0.9$$" %}
{% include figure.html path="../assets/c_learning/Ant-v2_gamma_0.99.gif" class="img-fluid rounded z-depth-1" caption="Ant-v2, $$\gamma = 0.99$$" %}

{% include figure.html path="../assets/c_learning/HalfCheetah-v2_gamma_0.50.gif" class="img-fluid rounded z-depth-1" caption="HalfCheetah-v2, $$\gamma = 0.50$$" %}
{% include figure.html path="../assets/c_learning/HalfCheetah-v2_gamma_0.90.gif" class="img-fluid rounded z-depth-1" caption="HalfCheetah-v2, $$\gamma = 0.90$$" %}

{% include figure.html path="../assets/c_learning/Hopper-v2_gamma_0.50.gif" class="img-fluid rounded z-depth-1" caption="Hopper-v2, $$\gamma = 0.50$$" %}
{% include figure.html path="../assets/c_learning/Hopper-v2_gamma_0.90.gif" class="img-fluid rounded z-depth-1" caption="Hopper-v2, $$\gamma = 0.90$$" %}

{% include figure.html path="../assets/c_learning/Walker-v2_gamma_0.50.gif" class="img-fluid rounded z-depth-1" caption="Walker-v2, $$\gamma = 0.50$$" %}
{% include figure.html path="../assets/c_learning/Walker-v2_gamma_0.90.gif" class="img-fluid rounded z-depth-1" caption="Walker-v2, $$\gamma = 0.90$$" %}
{% include figure.html path="../assets/c_learning/Walker-v2_gamma_0.99.gif" class="img-fluid rounded z-depth-1" caption="Walker-v2, $$\gamma = 0.99$$" %}

<!-- ![Ant-v2, $\gamma = 0.5$](images/Ant-v2_gamma_0.50.gif)
![Ant-v2, $\gamma = 0.9$](images/Ant-v2_gamma_0.90.gif)
![Ant-v2, $\gamma = 0.99$](images/Ant-v2_gamma_0.99.gif)
![HalfCheetah-v2, $\gamma = 0.5$](images/HalfCheetah-v2_gamma_0.50.gif)
![HalfCheetah-v2, $\gamma = 0.9$](images/HalfCheetah-v2_gamma_0.90.gif)
![Hopper-v2, $\gamma = 0.5$](images/Hopper-v2_gamma_0.50.gif)
![Hopper-v2, $\gamma = 0.9$](images/Hopper-v2_gamma_0.90.gif)
![Walker2d-v2, $\gamma = 0.5$](images/Walker2d-v2_gamma_0.50.gif)
![Walker2d-v2, $\gamma = 0.9$](images/Walker2d-v2_gamma_0.90.gif)
![Walker2d-v2, $\gamma = 0.99$](images/Walker2d-v2_gamma_0.99.gif) -->