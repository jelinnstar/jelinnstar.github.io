---
title: HotWireToolPathSrf
parent: ToolPath
layout: default
nav_order: 2
permalink: /en/05_HotWireToolPathSrf/
translation_link: /ko/05_HotWireToolPathSrf/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# HotWireToolPathSrf

## Description

* This component generates ToolPaths for hot wire cutting based on the input surface modeling data and related parameters.

<p align="center">  <img src="/assets/images/HotwireToolpathfromSrf.png" align="center" width="25%"></p>

## Input

* **Surface** : Specify the parameter for the surface to be cut using rib cutting. Only modeling data in the form of a Ruled Surface allows for the generation of rib cutting toolpaths.
* **Target Count** : Determines the number of planes that will compose the rib cutting toolpath.
* **Parameter** : Represents the normalized parameter value of RibCurve[MK1], determining the origin of the target. Only values between 0 and 1 can be input, and they can be applied sequentially within the specified Target Count. (Default: 0.5)

※ RibCurve refers to straight lines orthogonal to the base curve of the input Ruled Surface, which defines the rib cutting path. Each plane composing the rib cutting toolpath is generated based on points located on each RibCurve at the specified Parameter.

* **Wrist Object** : Utilizes modeling data such as points, curves, lines, etc., as attractors to redefine the normal direction of each Target Plane composing the rib cutting toolpath. This enables finding suitable robotic rib cutting operations.

### Built-in Param | Hotwire Srf

* **Cutting Direction Flip** : Reverses the direction of the rib cutting path.
* **Tool Flip** : Rotates the rib tool (end effector) by 180 degrees.
* **UV Flip** : If the input surface is a Ruled Surface in both U and V directions, this option allows switching the rib cutting direction to either the U or V direction.
* **Extension(mm)** : Adds additional target planes at a distance of Extension value from the surface modeling in the entry and exit directions of the rib cutting path.
* **Shift Seam** : Adjusts the starting position of the rib ToolPath to a specific location along the closed path (i.e., when the ToolPath forms a closed loop), based on a value between 0.0 and 1.0 derived from the input parameters.

### Built-in Param | Extra

* **NormalSize** : Adjusts the preview size of the ToolPaths.

## Output

* **Target Planes** : Outputs a list of planes that compose the rib ToolPaths.
* **RibCurves** : Outputs a list of RibCurves as Curve List.