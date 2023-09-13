---
layout: page
title: Contact-Implicit Optimization
description: How can we design robot behaviors that make and break contact? 
img: assets/img/12.jpg
importance: 1
category: work
related_publications: kurtz2023inverse, kurtz2022contact
---

Most things we want robots to do involve contact. Picking stuff up requires
contact. Moving around also requires contact (unless you can fly). 

But most robots today are bad at contact. Roboticists have spent a long time
thinking very hard about how to avoid contact entirely. And when contact is 
inevitable, as in manipulation and legged locomotion, we usually make strict assumptions
about where (feet only) when (following a predefined sequence) and how (softly
please!) contact occurs. Unsurprisingly, that can cause problems in the real
world.

Contact-implicit trajectory optimization aims to fix this by using numerical
optimization to decide when and where to make and break contact. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Whole-arm manipulation trajectories designed with contact-implicit
    optimization. The robot uses rich contact interactions along its whole arm
    to move the ball around. 
</div>

If we can solve contact-implicit optimization fast enough, we can use it for
real-time feedback via [Model Predictive
Control](https://en.wikipedia.org/wiki/Model_predictive_control) (MPC).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    MPC with contact-implicit optimization. The robot decides when and
    where to contact the box in real time.
</div>

