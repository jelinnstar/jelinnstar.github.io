---
title: Drawing
parent: ToolPath
layout: default
nav_order: 2
permalink: /en/00_Drawing/
translation_link: /ko/00_Drawing/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# Drawing

## Description

* This component generates a drawing ToolPath based on the input curve data and related parameters. Depending on whether Geometry Input is provided, it either creates a drawing ToolPath on a plane or generates a ToolPath that follows the shape of the Geometry.

<p align="center">  <img src="/assets/images/Drawing.png" align="center" width="25%"></p>

## Input

* **Curves[Curve / List]** : Select the curves to be drawn.
* **Reference Plane [Plane]** : Input the reference plane for drawing. The Target Plane is generated as a plane in the same xy direction as the Base Plane.
* **Geometry [Brep/Mesh / Optional]**: Input the geometry for the curves to be drawn on. Either a Mesh or Brep must be provided. The curves must be on the Geometry.

### Built in param | Drawing
  
  * **Tolerance** : Set the allowable tolerance.
  * **Min Edge(mm)** : Set the minimum distance between target planes. This parameter defines the minimum gap between parameters. Values smaller than this will not be generated.
  * **Max Edge(mm)** : Set the maximum distance between target planes. This parameter defines the maximum gap between parameters. Values larger than this will not be generated.
  * **Tilting Weight** : Set the degree to which the target plane tilts on the geometry. This is a normalized value (0-1) representing the tilt between the normal of the Base Plane and the normal of the target plane on the geometry.
  * **NormalSize** : Adjust the preview size of the ToolPaths.

## Output

* **Target Planes**: Output the defined Drawing ToolPath according to the given conditions.
