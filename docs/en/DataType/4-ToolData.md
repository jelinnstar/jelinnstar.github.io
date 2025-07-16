---
title: ToolData
parent: DataType
layout: default
nav_order: 2
permalink: /en/04-ToolData/
translation_link: /ko/04-ToolData/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# ToolData

## Description

* This component is mounted on the 6th axis of the robot and is responsible for providing and previewing information about the tool (end effector) to the robot.

<p align="center">  <img src="/assets/images/ToolData.png" align="center" width="25%"></p>

## Input

* **Name [Text/Item]** : Enter the unique variable name of the tool as a string.
* **Base Plane[Plane]** : Set the base plane of the tool mounted on the robot.
* **TCP [Plane]** : Set the reference plane representing the TCP of the mounted tool.

> Mass, Centroid, and Inertia should be entered based on the measurement results from the LoadIdentify Routine of the ABB robot system with the tool installed.

* **Mass [double/string]** : Enter the measured tool load. The maximum weight that is not recognized as a collision varies depending on the robot model. If the unspecified weight exceeds the default maximum weight, it will be recognized as a collision object and the operation will stop.
* **Centroid [Text/String]** : Enter the measured center of mass of the tool. The format should be 0d,0d,0d.
* **Inertia [Text/String]** : Enter the measured moment of inertia of the tool according to the robot's movement. The format should be 0d,0d,0d.
* **Export [Boolean]** : The user can save the entered tool information for future use.

### Built-in Param | Basic Params​

* **Display Colour** : Changes the color of the tool model.

<p align="center"> 
<video src="/assets/images/ToolData_Export.mp4" width="576px" height="324px" autoplay=1 muted=1 loop=1 align="center"></video>
</p>

## Output

* **ToolData** : Outputs the entered ToolData.
<p align="center">  <img src="/assets/images/ToolData_GIF_00-1.gif" align="center" width="100%"></p>
