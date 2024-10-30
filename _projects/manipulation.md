---
layout: page
title: Dextrous Manipulation
description: How can we get robots to move stuff around?
img: assets/img/allegro_rotation.gif
importance: 6
category: fun
related_publications: kurtz2023inverse, kurtz2020trajectory, kurtz2022contact,
    kurtz2021control, li2024drop
---

The goal of robot manipulation is simple: just move an object from point A to
point B. How hard could it be?

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/allegro_rotation.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/allegro_rotation_one.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/allegro_rotation_two.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A simulated robot hand uses <a href="https://idto.github.io">IDTO</a>
    to perform in-hand manipulation.
</div>

Very hard, it turns out. For example, consider the board games chess and Go.
These are very challenging games, with more possible games than atoms in the
universe, and computers are better than people at both. But in the
[famous](https://en.wikipedia.org/wiki/Deep_Blue_versus_Garry_Kasparov)
[matches](https://en.wikipedia.org/wiki/AlphaGo_versus_Lee_Sedol)
where computers first defeated the best human players, it was a
human engineer, not a robot, that moved the computer's pieces. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/DeepBlue_circled.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/AlphaGo_circled.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Computers can beat the best human players at chess and Go, but are still 
    <a href="https://www.theguardian.com/sport/2022/jul/24/chess-robot-grabs-and-breaks-finger-of-seven-year-old-opponent-moscow">
    not very good at moving the pieces</a>.
</div>

Dextrous manipulation is particularly difficult -- and fascinating -- because we humans are
so good at it. This can blind us to what we're actually doing. For example, 
early manipulation research focused a lot on grasping: how to
position the fingers around an object, how to plan a collision-free path to that
grasp, and so on.

Now there is a [growing
understanding](https://manipulation.csail.mit.edu/intro.html#section1)
that this may not be the best approach. When people move stuff around, we rarely search
for stable grasps. Instead, we push, pull, shuffle, and slide things into place,
constantly shifting between contact modes in complicated and interesting ways. 

## Image Sources

1. [https://www.pri.org/stories/2018-01-05/garry-kasparov-and-game-artificial-intelligence](https://www.pri.org/stories/2018-01-05/garry-kasparov-and-game-artificial-intelligence)
2. [https://www.theguardian.com/technology/2016/mar/09/google-deepmind-alphago-ai-defeats-human-lee-sedol-first-game-go-contest](https://www.theguardian.com/technology/2016/mar/09/google-deepmind-alphago-ai-defeats-human-lee-sedol-first-game-go-contest)
