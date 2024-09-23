---
layout: page
title: Machine Learning
description: Can we combine the promise of machine learning with the rigor of model-based control?
img: assets/img/neural_net.png
importance: 4
related_publications: saxena2016learning, kurtz2019toward, lemmon2022learning,
    kurtz2022mini
---

Deep neural networks have revolutionized computer vision and natural language
processing, solving problems that [previously seemed
intractable](https://xkcd.com/1425/). Is robotics next?

It's possible, but there are a few major hurtles. One is
data: unlike computer vision and natural language processing, the internet does
not contain vast troves of ready-made robotics data. Collecting new data is slow
and expensive, especially if hardware experiments are involved. Another problem is 
safety. Machine learning methods can perform well, but they
don't generalize outside the training dataset and can sometimes exhibit
[surprisingly bad
behaviors](https://ieeexplore.ieee.org/abstract/document/8294186).

One potential solution is to combine machine learning with classical model-based control. 
Ideally, this can bring together the best of both worlds. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/falling_cat_1.jpg" title="falling cat frame" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/falling_cat_2.jpg" title="falling cat frame" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/falling_cat_3.jpg" title="falling cat frame" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/falling_cat_4.jpg" title="falling cat frame" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    To land a quadruped robot on its feet like a cat, we combined
    supervised learning and model-based trajectory optimizaiton.
</div>

Additionally, there's good reason to hope that model-based techniques can
inspire the next revolution in machine learning for robotics. Contrary to a
popular narrative about the "magic" of deep learning, recent breakthroughs in
computer vision and natural language processing were enabled by key insights into
the structure of the problem. For computer vision, this insight was the 
importance of
[convolution](https://en.wikipedia.org/wiki/Convolutional_neural_network). 
For natural language, it was the concept of 
[attention](https://en.wikipedia.org/wiki/Transformer_(machine_learning_model)).
What is the key structural insight that will enable machine learning for robotics 
at scale?

