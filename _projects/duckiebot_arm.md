---
layout: page
title: Duckiebot Arm
description: Collaboration with Duckietown. World's smallest fully-programmable mobile manipulator.
img: assets/img/projects/duckiebot-arm/cover.jpg
importance: 4
category: robotics
redirect:
related_publications: false
---
<hr>
<div class="row">
    <div class="col">
        {% include video.liquid path="assets/img/projects/duckiebot-arm/grasp_duck.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true muted=true loop=true %}
    </div>
</div>

I had the pleasure of designing and building a 4-DOF prototype arm module with [Duckietown](https://duckietown.com/), a company offering small autonomous vehicles ("Duckiebots") for education and research. The arm enables the Duckiebot to grasp objects and interact with its environment, leading to a wide range of new applications. With the arm module, the Duckiebot is among the world's smallest fully-programmable mobile manipulators.

<div class="row">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/projects/duckiebot-arm/camera.jpg" title="Palm camera" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/projects/duckiebot-arm/camera_stream.jpg" title="Camera stream" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="caption">
    The Duckiebot Arm features a palm camera with 30 FPS 2592 × 1944 resolution.
</div>

I used a combination of 3D printing and off-the-shelf components to build the arm. The servos are [Dynamixel XL330-M288](https://emanual.robotis.com/docs/en/dxl/x/xl330-m288/), which offer six different control modes. The arm features a 2592 × 1944 pixel [palm camera](https://www.waveshare.com/wiki/IMX335_5MP_USB_Camera_(B)) streaming up to 30 FPS. A comparison between the [Duckiebot](https://get.duckietown.com/products/duckiebot-db21) and the Duckiebot with arm module is shown below.

<div class="row">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/projects/duckiebot-arm/comparison.jpg" title="Duckiebot Comparison" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
<div class="caption">
    Comparison between the <a href="https://get.duckietown.com/products/duckiebot-db21">Duckiebot</a> and the Duckiebot prototype with arm module.
</div>
