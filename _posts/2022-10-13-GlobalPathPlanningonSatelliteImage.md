---
layout: post
title: Global path planning based on satellite images
date: 2022-10-13
comments: true
description: Traditional RRT* and GAIl.
thumbnail: assets/img/post2-0.jpg
---

Based on satellite imagery, the Sat2Graph [1] method is used to automatically generate an initial road network. This initial road network is then manually corrected and refined to obtain the final road network result.

On the basis of this final road network, traditional planning method (RRT* in OMPL) [2] are used to generate planning results, forming a dataset. This dataset is then used to train an imitation learning model [3].

Finally, the imitation learning model is applied for planning. This imitation learning approach yields faster planning results at a large scale (20km) compared to using traditional planning method alone.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/post2-2.jpg" title="vehicle" class="img-fluid rounded z-depth-1" zoomable=true %} 
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/post2-1.jpg" title="vehicle" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="caption">
    RRT* planner visulization and Planning software GUI.
</div>

[1] He, Songtao, et al. "Sat2graph: Road graph extraction through graph-tensor encoding." Computer Vision–ECCV 2020: 16th European Conference, Glasgow, UK, August 23–28, 2020, Proceedings, Part XXIV 16. Springer International Publishing, 2020.

[2] Ioan A. Șucan, Mark Moll, Lydia E. Kavraki, The Open Motion Planning Library, IEEE Robotics & Automation Magazine, 19(4):72–82, December 2012. https://ompl.kavrakilab.org 

[3] Ho, Jonathan, and Stefano Ermon. "Generative adversarial imitation learning." Advances in neural information processing systems 29 (2016).

