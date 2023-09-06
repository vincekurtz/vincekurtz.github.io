---
layout: page
title: Machine Learning
description: Can we combine the promise of machine learning and the rigor of model-based method?
img:
importance: 4
related_publications: saxena2016learning, kurtz2019toward, lemmon2022learning,
    kurtz2022mini
---

Deep neural networks have revolutionized computer vision and natural language
processing, solving problems that previously seemed intractable. Is robotics
next?

It's possible, but there are still a few major hurtles. One is
data: unlike computer vision and natural language processing, the internet does
not contain vast troves of ready-made robotics data. Collecting new data is slow
and costly, especially if hardware experiments are involved. 

Another problem is safety. Machine learning methods can perform well, but they
don't generalize outside the training dataset and can sometimes exhibit
surprisingly bad behaviors. 

A potential solution to both these problems is to combine ML methods with
classical model-based control. Ideally, this can bring together the best of both
worlds. 

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
    To land a quadruped robot on its feet like a cat, we used a combination of
    supervised learning and model-based trajectory optimizaiton.
</div>
