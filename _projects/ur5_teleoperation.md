---
layout: page
title: UR5 Teleoperation
description: UR5 teleoperation with Leap Motion hand-tracking and Meta Quest 3. Showcased at MSI in Chicago, 2024.
img: assets/img/projects/ur5-teleoperation/cover.jpg
importance: 2
category: robotics
redirect:
related_publications: false
---
<hr>

With the help of lab members at TTIC, I implemented two teleoperation systems for our lab's UR5 robot: one with [Leap Motion](https://www.ultraleap.com/) hand-tracking and another with [Meta Quest 3](https://www.meta.com/quest/quest-3/). This was the first teleoperation system in our lab, and was showcased at the Museum of Science and Industry in Chicago in April 2024.

<div class="row">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/projects/ur5-teleoperation/msi.jpg" title="MSI Demo" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
    <div class="col">
        {% include video.liquid path="assets/img/projects/ur5-teleoperation/msi_cups.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true muted=true loop=true %}
    </div>
</div>
<div class="caption">
    Showcasing UR5 teleoperation with <a href="https://www.ultraleap.com/">Leap Motion</a> hand-tracking at the Museum of Science in Chicago, April 2024.
</div>

The Leap Motion controller was used to track hand movements and gestures, which were then mapped to the UR5 robot's end-effector. I had to ensure that the robot's movements were smooth and robust to rapid or jerky hand movements. This was achieved using smoothing, velocity and acceleration clipping, and tuning the PID controller. The Leap Motion teleoperation gained popularity at the museum, with visitors trying to hang mugs on a rack.

<div class="row">
    <div class="col">
        {% include video.liquid path="assets/img/projects/ur5-teleoperation/blocks.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true muted=true loop=true %}
    </div>
    <div class="col">
        {% include video.liquid path="assets/img/projects/ur5-teleoperation/water.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true muted=true loop=true %}
    </div>
    <div class="col">
        {% include video.liquid path="assets/img/projects/ur5-teleoperation/dishwasher.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true muted=true loop=true %}
    </div>
</div>
<div class="caption">
    Real-time block-stacking, water pouring, and dishwasher loading tasks with <a href="https://www.meta.com/quest/quest-3/">Meta Quest 3</a> teleoperation.
</div>

Leap Motion teleoperation was not intuitive enough for large-scale collection of demonstrations. Thus, I implemented a second teleoperation system using the Meta Quest 3 VR headset. The Quest controller's linear and angular velocities were mapped to the UR5's end-effector, so the user can control the robot from anywhere in the room. This system enabled lab members to efficiently collect demonstrations of challenging and dextrous tasks for imitation learning.
