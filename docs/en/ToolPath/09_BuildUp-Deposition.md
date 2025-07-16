---
title: BuildUp Deposition
parent: ToolPath
layout: default
nav_order: 2
permalink: /en/09_BuildUp-Deposition/
translation_link: /ko/09_BuildUp-Deposition/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# BuildUp Deposition

## Description

* Component for analyzing additive manufacturing (AM) data to assist in generating general deposition toolpaths.

<p align="center">  <img src="/assets/images/BuildupDeposiiton.png" align="center" width="25%"></p>

## Input

* **Home Pos [Plane/Optional]**: Input the plane corresponding to the home position before deposition starts. Default value is World XY.
* **Deposition ToolPaths [DepositionToolPath / List]**: Receives DepositionToolPath data.
* **Pre-Extrusion Curve [Curve/Optional]**: Optional curve data for nozzle cleaning by pre-extrusion.
* **Is Bottommost [Boolean]**: Checks if the deposition toolpath starts from the bottommost layer.

## Output

* **E-Start Planes**: Outputs the first plane value of the main path where extrusion begins.
* **Movement Planes**: Outputs the plane values along the main path where extrusion is carried out.
* **E-Stop Planes**: Outputs the plane value where extrusion stops along the main path.
* **E-Stop idx**: Outputs the index of the E-Stop plane.