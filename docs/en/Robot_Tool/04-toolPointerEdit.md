---
title: ToolPointerEdit
parent: Robot/Tool
layout: default
nav_order: 2
permalink: /en/04-toolPointerEdit/
translation_link: /ko/04-toolPointerEdit/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# ToolPointerEdit

## Description

* This component assists in configuring the spindle tool. It takes the modeling (Mesh) of the spindle body and the point corresponding to the starting point of the end mill (Plane) as inputs. It then exports the TCP value based on the length and diameter of the end mill.
Considering models with and without the end mill included, it allows for setting the length, size, and direction of the TCP accordingly.

<p align="center">  <img src="/assets/images/ToolPointEdit.png" align="center" width="25%"></p>

## Input

* **Tool Geometry [Mesh]** : Input the mesh of the spindle body.
* **Endmill StartPl [Plane]** : Input the plane where the end mill attaches, similar to the TCP (Tool Center Point).

### Built-in Param : Basic Params

* **Length(mm)** : Determines the length of the end mill in millimeters (mm).
* **Radius(mm)** : Determines the radius of the end mill's diameter in millimeters (mm).

## Output

* **Tool Geometry** : Exports the spindle body mesh as the ToolData mesh.
* **TCP** : Exports the plane at the end of the end mill's final length and radius, as configured by the user, as the TCP.

<p align="center"> 
<video src="/assets/images/spindleEditor_source1.mp4" width="576px" height="324px" autoplay=1 muted=1 loop=1 align="center">
</video>
</p>

