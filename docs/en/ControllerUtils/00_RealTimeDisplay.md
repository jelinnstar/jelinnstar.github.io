---
title: RealTimeDisplay
parent: Controller Utils
layout: default
nav_order: 2
permalink: /en/00_RealTimeDisplay/
translation_link: /ko/00_RealTimeDisplay/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# RealTimeDisplay

## Description

* RealTimeDisplay is a component that connects with the actual or virtual robot ID, allowing you to observe the movements of the connected robot synchronized with the GERTY simulation movements

<p align="center">  <img src="/assets/images/realtimedisplay.png" align="center" width="40%"></p>

## Input

* **GERTY Robot**: Receive robot component data.
* **SystemID** : Receive robot controller data.

### Built-in Param | CurrentTCP
* **Types**: Reads data from the components installed on the actual robot. Default value is 'Tool'.
* **Options**: Choose output options for robot data.

## Output

* **Robot Angle** : Fetches and displays the angle values for each axis of the robot.
* **External Angle** : Fetches and displays the angle values of the additional axes.
* **CurrentPos**: Outputs the current pose of the robot.

## How To Use

The following examples illustrate typical usage scenarios of the `RealTimeDisplay` component.

<p align="center">  <img src="/assets/images/RealTimeDisplay_00-768x249.png" align="center" width="90%"></p>

<p align="center"> 
<video src="/assets/images/IMG_0556-2.mp4" width="576px" height="324px" autoplay=1 muted=1 loop=1 align="center">
</video>
</p>


