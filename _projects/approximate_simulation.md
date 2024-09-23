---
layout: page
title: Certifying Reduced-Order Models
description: Can we obtain formal guarantees when planning with a reduced-order model?
img: assets/img/7.jpg
importance: 3
category: work
related_publications: kurtz2020approximate, song2022robust,
    kurtz2020robust, kurtz2021control, kurtz2019formal
---

[All models are wrong, but some models are
useful](https://en.wikipedia.org/wiki/All_models_are_wrong).
In many robotics applications, rigid-body dynamics are the model of choice.
Rigid-body dynamics are fairly accurate for robots like quadrupeds, humanoids,
and manipulators, but they are often too complicated to be useful. 

Often roboticists use even simpler models to design controllers, especially for
legged locomotion.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Popular reduced-order models for legged locmotion: the Linear Inverted
    Pendulum (LIP), Spring Loaded Inverted Pendulum (SLIP), and compass-gait walker. 
</div>

These reduced-order models capture only the most relevant features of the
dynamics, such as the relationship between foot placement and the
center-of-mass. These models underpin much of the success of walking robots in
recent years.

But there is a large gap between these reduced-order models and more complete
rigid-body models, not to mention the actual physics of the robot. How can we be
sure that a plan generated with a reduced-order model actually feasible? Can we
provide some performance guarantees when we use a reduced-order model?

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The framework of <em>approximate simulation</em> enables formal guarantees when 
    planning with a reduced-order model. This also improves controller performance. 
</div>

