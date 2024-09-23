---
layout: page
title: Temporal Logic Planning
description: How can robots plan to accomplish complex tasks?
img: assets/img/large_door_puzzle_scenario.png
importance: 2
category: work
related_publications: kurtz2023temporal, kurtz2022mixed, kurtz2021scalable,
    silva2021automatic, silva2021symbolic, kurtz2020trajectory,
    gilpin2020smooth, silva2019active
---

Roboticists and control theorists have a few favorite problems: Reach a goal
while avoiding obstacles. Stabilize a fixed-point. Find
a minimum-cost control action. But
many of the tasks that we want robots to do in the real world don't fit 
neatly into any of these formulations. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        {% include figure.html path="assets/img/large_door_puzzle_scenario.png" title="door puzzle scenario" width="50%" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    An example of a more complex task: starting from the "x", a robot must
    reach the goal (blue), but before passing through each door (red) it
    must first pick up a corresponding key (green). 
</div>

Temporal logic is one way to specify a wide array of desired behaviors. 
Given a logical formula that defines the task, how can we generate a trajectory 
that satisfies the specification? Can we guarantee that our algorithm will find
a solution if one exists? 

Temporal logic planning is 
[NP-hard](https://en.wikipedia.org/wiki/NP-hardness), so there is a
significant tradeoff between completeness and computational efficiency. 

