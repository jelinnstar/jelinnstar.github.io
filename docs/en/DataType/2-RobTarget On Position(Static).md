---
title: RobTarget On Position(Static)
parent: DataType
layout: default
nav_order: 2
permalink: /en/02-RobTarget On Position(Static)/
translation_link: /ko/02-RobTarget On Position(Static)/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# RobTarget On Position(Static)

## Description

* The Positioner's RobTarget (Robot Target) is a component that defines the position of the robot and additional axes using user-defined ToolPath Plane data to define the RobTarget data. 
* RobTarget On Positioner is a data format in the ABB RAPID Program that defines the movements of the robot and auxiliary equipment. 
* RobTarget On Positioner includes information such as the position and orientation of the robot's TCP (Tool Center Point) and the angle information of the additional axes along the planned movement path.
  * Reference: ABB RAPID Instructions Documentation (Document ID: 3HAC050917-001).

<p align="center">  <img src="/assets/images/positioner_static.png" align="center" width="25%"></p>

## Input

* **Positioner** : Inputs Positioner Data.
* **Name [Text/Item]** : Specify the variable name of the ABB RobTarget as a string.
* **Target Plane [Plane/DataTree]** : Receives data for the ToolPath Plane planned by the user.
* **Base Plane [Plane/DataTree]** : Receives data for the ToolPath Plane planned by the user.
* **Reference Plane [Plane/DataTree]** : Inputs the reference Plane value for each branch of the Target Plane.
* **Angle [Number/Item]** : Modifies the robot's posture by changing the angle of the TargetPlane's normal.
* **WobjData [Plane]** : Defines the reference plane according to the workspace as Work Object Data.

<p align="center"> 
<video src="/assets/images/RobtargetPosition_Static_Top.mp4" width="576px" height="324px" autoplay=1 muted=1 loop=1 align="center"><figcaption>Top View</figcaption>
</video></p>


### Built-in Param | Basic Params​

* **Split Start** : Can split the first TargetPlane Data of the TargetPlane. The default state is False.
* **Split End** : Can split the last TargetPlane Data of the TargetPlane. The default state is False.

<br>

## Output

* **RobTargets** : Print ProgramData of Robtargets in each area. Then, link this data to Instructions.

<p align="center"> 
<video src="/assets/images/Static_RobPosition_gif.mp4" width="576px" height="324px" autoplay=1 muted=1 loop=1 align="center">
</video>
</p>