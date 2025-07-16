---
title: Move
parent: Instruction
layout: default
nav_order: 2
permalink: /en/02-Move/
translation_link: /ko/02-Move/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# Move

## Description

* To facilitate TCP movement, this component defines the Move Instruction by receiving RobTarget data. The movements for each target can be configured with Type, Speed, and Zone options.

<p align="center">  <img src="/assets/images/Move_2.png" align="center" width="25%"></p>

## Input

* **RobTargets** : Receives the data of RobTargets.

### Built-in Param | Move

* **MoveJ** : Move Joint, where the robot reaches the Target Plane in regular kinematics, interpreted as the optimal posture.
* **MoveL** : Move Linear, where the robot reaches the Target Plane in inverse kinematics from a user-defined posture, finding the shortest path.
* **Speed** : Sets the speed (velocity) in mm/s at which the RobTarget is reached.
* **Zone** : Specifies a radius around the Target Point. When moving to the next Target Point, the movement is controlled by filleting with a size proportional to the zone value. This ensures precise passage through the point, while potentially affecting the robot's constant speed motion.


<p align="center"> 
<video src="/assets/images/Move_gif_confirm-min_SHL.mp4" width="576px" height="324px" autoplay=1 muted=1 loop=1 align="center"></video>
</p>

## Output

* **Instructions** : Outputs the defined Move Instructions based on the entered Input.
