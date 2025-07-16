---
title: Positioner
parent: Robot/Tool
layout: default
nav_order: 2
permalink: /en/02-Positioner/
translation_link: /ko/02-Positioner/
nav_exclude: true
---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# Positioner

## Description

* This is a component that allows for user-defined modeling of ABB Positioner models.

<p align="center">  <img src="/assets/images/Positioner.png" align="center" width="25%"></p>

## Input

* **Name [Text]** : Allows setting a unique name for the Positioner. If not set, the default value will be STN1.
* **PositionerFCPL [Plane]**: Stands for Positioner Flange Center Plane, allowing you to input the center plane of the positioner flange.
* **WorkBench [WorkBench Data]** : Allows you to input the workbench modeling for the Positioner.

### Built-in Param : Preview Params​

* **Model** : Specifies the positioner model.
* **Positioner Colour** : Redefines the color of the positioner model.

### Built-in Param : Vector Params​

* **Enable Arm** : Allows you to lock the position of the positioner. By default, the positioner arm is unlocked.
* **Approaching Dir.** : Redefines the direction of the approach path to the positioner.
* **TCP Dir.** : Redefines the direction of the TCP (Tool Center Point) approach to the positioner.

## Output

* **GERTY Positioner** : Exports the information of the user-defined positioner.
* **Arm** : Exports the coordinate values of the current position of the robot arm.
* **Plate** : Exports the coordinate values of the current plane of the robot workbench.
* **ConnectPl** : Outputs the coordinate plane linking the robot workbench and the positioner.


<p align="center"> 
<video src="/assets/images/Workbench_gif.mp4" width="576px" height="324px" autoplay=1 muted=1 loop=1 align="center">
</video>
</p>