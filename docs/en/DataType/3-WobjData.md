---
title: WobjData
parent: DataType
layout: default
nav_order: 2
permalink: /en/03-WobjData/
translation_link: /ko/03-WobjData/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# WobjData

## Description

* WobjData is a component that defines the internal work object of a robot.
It allows transforming the position of the internal work object from WobjData to a user-defined UserFrame, and can be adapted to the robot's model and additional axes by changing to Fixed WobjData and MovableData.

<p align="center">  <img src="/assets/images/04_WobjData.png" align="center" width="25%"></p>

## Input

* **Name [Text]** : Enter the variable name for the UserFrame.
* **UserFrame [Plane]** : Set the Base Plane.

### Felxible Option

* **Fixed WobjData** : Redefines the Target Plane relative to a stationary reference coordinate system.
* **Movable WobjData** : Redefines the Target Plane relative to a movable (dynamic) reference coordinate system.

<p align="center">  <img src="/assets/images/wobj_movable.png" align="center" width="45%"></p>


## Output

* **WobjData** : Outputs the defined WobjData.
