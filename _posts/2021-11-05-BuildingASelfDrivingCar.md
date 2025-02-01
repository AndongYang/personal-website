---
layout: post
title: Building a self-driving car
date: 2021-11-05
comments: true
description: Sensor installation and path planning software design.
thumbnail: assets/img/f51.jpeg
---

Building a self-driving car that drives in the plateau environment. Participate in vehicle modification and solve the problem of no HD map, irregular path, and difficulty in manually correcting the path faced by global path planning for vehicle in plateau environment. Specific details include:
* Drawing the road network based on satellite images; 
* Global path planning based on RRT* and A*.
* A visual interface based on QT is written to set target and check or modify the planning results.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/f51.jpeg" title="vehicle" class="img-fluid rounded z-depth-1" zoomable=true %} 
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/f52.png" title="vehicle" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="caption">
    Modified vehicle.
</div>

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/post1-1.jpg" title="vehicle" class="img-fluid rounded z-depth-1" zoomable=true %} 
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/post1-2.jpg" title="vehicle" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="caption">
    Path Planning software.
</div>


