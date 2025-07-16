---
title: MoveXO
parent: Instruction
layout: default
nav_order: 2
permalink: /en/03-MoveXO/
translation_link: /ko/03-MoveXO/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# Move

## Description

* To enable TCP movement, this component generates move instructions by processing RobTarget data. Each target’s motion can be configured using parameters such as Type, Speed, and Zone.

<p align="center">  <img src="/assets/images/MoveXO.png" align="center" width="25%"></p>

# Input

* **RobTargets** : Receives a list of RobTarget data.
* **Signal** : Specify the exact name of the signal used.
* **DO Value [Boolean]** : Set the output state as either True or False.

## Built-in Param | Move

* **MoveJDO** : Digital Output, Move Joint — moves the robot to the Target Plane using forward kinematics, selecting the optimal posture calculated by the robot.
* **MoveLDO** : Digital Output, Move Linear — moves to the Target Plane using inverse kinematics from the user-defined posture, taking the shortest path.
* **MoveJGO** : Group Output, Move Joint — same as MoveJDO but for grouped outputs.
* **MoveLGO** : Group Output, Move Linear — same as MoveLDO but for grouped outputs.
* **MoveJAO** : Analog Output, Move Joint — same as MoveJDO but for analog outputs.
* **MoveLAO** : Analog Output, Move Linear — same as MoveLDO but for analog outputs.
* **Speed** : Sets the travel speed toward each RobTarget in millimeters per second (mm/s).
* **Zone** : Defines the blending radius at each target point. When transitioning to the next point, the robot path is smoothed (filleted) based on the zone value. Fine forces the robot to pass exactly through the point but may affect velocity consistency.

## Built-in Param | MoveXO

* **MoveJXO Start&End** : Fixes both the start and end of the Target Plane to a Move Joint motion.
* **Fine Start&End** : Fixes both the start and end of the Target Plane to Fine positioning (zero radius), ensuring precise arrival at the point.


# Output

* **Instructions** : Outputs a set of MoveXO instructions based on the provided inputs and motion configuration.