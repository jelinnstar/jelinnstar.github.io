---
title: ObjRoughing
parent: ToolPath
layout: default
nav_order: 2
permalink: /en/06_ObjRoughing/
translation_link: /ko/06_ObjRoughing/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# ObjRoughing

## Description

* Component providing cutting toolpaths for the first milling stage.

<p align="center">  <img src="/assets/images/ObjRoughing.png" align="center" width="25%"></p>

## Input

* **Geometry**: Input the volume to be roughed out as a solid (Brep) or mesh (Mesh) type.
* **Reference Plane** : Input the reference plane that determines the end mill entry direction (Contour direction), target orientation, starting position of the toolpath, collision avoidance height for machining surfaces, etc.

### Built-in Param | Roughing

* **Cutting Direction [Boolean]**: Selects the upward (True) or downward (False) cutting direction.
* **Setback** : Determines the extent to which the roughing toolpath is offset from the final machined surface. It must be greater than half the diameter of the end mill. (Setback > End mill diameter * 1/2)
* **Stepover**: Specifies the amount of horizontal material removed in one pass, calculated as less than half the diameter of the end mill. (Stepover <= End mill diameter * 1/2)
* **Stepdown**: Sets the vertical depth of each drilling pass, calculated as less than half the flute length of the end mill. (Stepdown <= End mill flute length * 1/2)
* **Shift**: Shifts the entire vertical direction of the Stepdown layer.
* **Tolerance**: Determines the resolution of the toolpath.

## Output

* **Targets Plane** : Converts the results of movement and avoidance paths into a DataTree with even branches.
* **ToolPath** : Converts the results of movement and avoidance paths into a DataTree with even branches.