---
title: ScanToolData
parent: Controller Utils
layout: default
nav_order: 2
permalink: /en/03_ScanToolData/
translation_link: /ko/03_ScanToolData/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# ScanToolData

## Description

* ScanToolData is a component that assists in extracting current tool data information from virtual or real robots.

<p align="center">  <img src="/assets/images/ScanToolData.png" align="center" width="25%"></p>

## Input

* **SystemID** : Enter the ID of the robot currently connected to the controller.

## Output

* **ToolName** : Outputs the name of the tool connected to the current controller.
* **TCP** : Outputs the TCP data of the robot connected to the current controller.
* **Mass** : Outputs the tool weight data of the robot connected to the current controller. 
* **Centroid** : Outputs the Centroid value of the tool connected to the current controller. 
* **Inertia** : Outputs the Inertia value of the tool connected to the current controller.

## How To Use

* Read the current robot ID using ScanABBController and connect it to ScanToolData for use. Extract the tool data of the robot to assist with precise simulation.
<p align="center">  <img src="/assets/images/RealTimeDisplay_01-768x341 (1).png" align="center" width="90%"></p>
