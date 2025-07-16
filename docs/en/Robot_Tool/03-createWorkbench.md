---
title: CreateWorkbench
parent: Robot/Tool
layout: default
nav_order: 2
permalink: /en/03-createWorkbench/
translation_link: /ko/03-createWorkbench/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# Positioner

## Description

* This is a component that allows for user-defined modeling of the workbench.

<p align="center">  <img src="/assets/images/Workbench.png" align="center" width="25%"></p>

## Input

* **WorkBenchMesh** : Receives the user-defined or existing workbench modeling mesh.
* **WorkBenchBasePl** : Sets the base plane for the workbench modeling.
* **WorkBenchFCPl** : Sets the flange center plane for the workbench.
* **Export [Boolean]** : Allows the user to save the workbench.

<p align="center"> 
<video src="/assets/images/Workbench_Export.mp4" width="576px" height="230px" autoplay=1 muted=1 loop=1 align="center"></video><figcaption>Workbench Export</figcaption>
</p>

### Built-in Param : Basic Params

* **Display Colour** : Sets the color of the robot model.
* **Objs Colour** : Sets the color of the objects.

## Output

* **GERTY Workbench**: Exports the information of the user-defined workbench.