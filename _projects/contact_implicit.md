---
layout: page
title: Contact-Implicit Optimization
description: How can we design trajectories that make and break contact? 
img: assets/img/lift_simulation.png
importance: 1
category: work
related_publications: kurtz2023inverse, kurtz2022contact
---

Most things we want robots to do involve contact. Picking stuff up requires
contact. Moving around also requires contact (unless you can fly). 

But most robots today are bad at contact. Roboticists have spent a long time
thinking very hard about how to avoid collisions entirely. And when contact is 
inevitable, as in manipulation and legged locomotion, we usually make strict assumptions
about where (feet only) when (following a predefined sequence) and how (softly
please!) contact occurs. Unsurprisingly, that can [cause problems](https://youtu.be/g0TaYhjpOfo) 
in the real world.

Contact-implicit trajectory optimization aims to fix this by using numerical
optimization to decide when and where to make and break contact. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/forward_push_frames.png" title="robot rolls a ball" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A whole-arm-manipulation trajectory designed with contact-implicit
    optimization. The robot uses rich contact interactions along its arm to move the ball. 
</div>

If we can solve contact-implicit optimization quickly and reliably, we can use it for
real-time feedback via [Model Predictive
Control (MPC)](https://en.wikipedia.org/wiki/Model_predictive_control).

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="assets/video/bimanual_strike.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true %}
    </div>
</div>
<div class="caption">
    MPC with contact-implicit optimization. The robot decides when and
    where to contact the box in real time.
</div>

Doing so is easier said than done. Contact introduces a slew of numerical and
modeling challenges, and general-purpose optimizers are typically not up to the
task. Additionally, contact-implicit optimization is highly nonlinear with many
local minima. Finding a globally optimal solution is 
[NP-hard](https://en.wikipedia.org/wiki/NP-hardness),
and is probably too much to ask. Even finding a good-enough local optimum 
can be very difficult.

