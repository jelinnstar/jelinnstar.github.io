---
title: ReadAndWriteMOCData
parent: Controller Utils
layout: default
nav_order: 2
permalink: /en/02_ReadAndWriteMOCData/
translation_link: /ko/02_ReadAndWriteMOCData/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# ReadAndWriteMOCData

## Description

* ReadAndWriteMOCData is a component that outputs the information of the virtual or real positioner axis connected to the current controller.

<p align="center">  <img src="/assets/images/ReadAndWriteMOCData.png" align="center" width="25%"></p>

## Input

* **SystemID** : Receives robot controller data.

## Output

* **ARM1&PLATE1_Info** : Outputs the axis values of ARM1 and PLATE1 of the positioner. 
* **PLATE_Pl** :  Outputs the table plane position value of the positioner. 
* **ARM1_Pl** : Outputs the position value of the ARM1 axis plane of the positioner.

<p align="center">  <img src="/assets/images/ReadAndWriteMOCData_01-1-768x272.png" align="center" width="90%"></p>

## How To Use

* The following is an example you may encounter when using the ReadAndWriteMOCData component.

<p align="center">  <img src="/assets/images/ReadAndWriteMOCData_02-1-768x184.png" align="center" width="90%"></p>