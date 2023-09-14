---
layout: page
title: Certifying Reduced-Order Models
description: Can we obtain formal guarantees when planning with a reduced-order model?
img: assets/img/slip_model.png
importance: 3
category: work
related_publications: kurtz2020approximate, song2022robust,
    kurtz2020robust, kurtz2021control, kurtz2019formal
---

[All models are wrong, but some models are
useful](https://en.wikipedia.org/wiki/All_models_are_wrong).
In many robotics applications, rigid-body dynamics are the model of choice.
Rigid-body models are fairly accurate for robots like quadrupeds, humanoids,
and manipulators, but they are often too complicated to be useful. 

This leads roboticists use simpler models to design controllers, especially for
legged locomotion.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/lip_model.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/slip_model.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/compass_gait.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Popular reduced-order models for legged locmotion: the linear inverted
    pendulum, spring loaded inverted pendulum, and compass-gait walker. 
</div>

These reduced-order models capture only a few key features of the
dynamics, such as the relationship between foot placement and the
center-of-mass. Simplified models underpin much of the success of walking robots in
recent years.

But there is a large gap between these reduced-order models and more complete
rigid-body models, not to mention the actual physics of the robot. How can we be
sure that a plan generated with a reduced-order model is actually feasible? Can we
provide some performance guarantees when we use a reduced-order model?

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="assets/video/RAL2020_summary.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true loop=true %}
    </div>
</div>
<div class="caption">
    The framework of <em>approximate simulation</em> enables formal guarantees
    for humanoid locomotion using a reduced-order model.
</div>

