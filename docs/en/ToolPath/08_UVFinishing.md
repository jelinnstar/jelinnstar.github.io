---
title: UVFinishing
parent: ToolPath
layout: default
nav_order: 2
permalink: /en/08_UVFinishing/
translation_link: /ko/08_UVFinishing/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# UVFinishing

## Description

* 2nd Milling Stage Cutting Toolpath Component: Outputs values that divide curves parallel between curves of different lengths in the direction of the Cutting Direction, as shown in the figure below.

<p align="center">  <img src="/assets/images/UV_Finishing.png" align="center" width="25%"></p>

## Input

* **Brep**: Input a Brep or Surface UV object.
* **Reference Plane**: Input the reference plane for Target Orientation when Tilting weight = 0.

<p align="center"><img src="/assets/images/UVfinishing-768x238.png" align="center" width="80%"></p>

### Built-in Param | UVFinishing

* **Cutting Direction [Boolean]**: Select the direction – U (False) / V (True).
* **Stepover**: Determines the amount of material removed in the horizontal direction. The default value is less than or equal to half the end mill diameter, allowing for finer finishing. (Stepover <= End Mill Diameter * 1/2)
* **Tilting Weight**: Weight for Target Tilting, accepts values between 0.0 and 1.0. Closer to 0 means the Target Plane aligns with the normal of the Base Plane; closer to 1 means it aligns with the normal of the Surface.
* **Tolerance**: Toolpath resolution.

## Output

* **Curve**: Outputs the curves of the finishing layer.
* **Target Plane**: Outputs the indices of planes as a DataTree.