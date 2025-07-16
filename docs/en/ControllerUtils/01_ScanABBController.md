---
title: ScanABBController
parent: Controller Utils
layout: default
nav_order: 2
permalink: /en/01_ScanABBController/
translation_link: /ko/01_ScanABBController/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# ScanABBController

## Description

* This is a component that searches for a robot controller compatible with wired or wireless connection on the GERTY-operated PC.

<p align="center">  <img src="/assets/images/ScanABBController.png" align="center" width="25%"></p>

## Input

* **Update[Boolean/Item]**: Updates information on available controllers that can be connected.

### Built-in Param | Controller
* **Controller Type**: Allows selection between virtual (Virtual) and physical (Real) robot environments.

<div align="center">
<table style="border-collapse: collapse: width: 51 %; height: 100px;" border="0.5" data-ke-style="sytle4">
<tbody>
<tr style="height: 20px;" bgcolor="#F2F2F2">
<td style="width: 45%; height: 20px; text-align: center; font-weight: bolder;">Virtual</td>
<td style="width: 50%; height: 20px; text-align: center; font-weight: bolder;">Real</td>
</tr>
<tr style="height: 0px;">
<td style="width: 50%; height: 1-px; text-align: left;" rowspan="1">By connecting to the virtual robot controller in ABB RobotStudio, you can retrieve the necessary data and control GERTY.</td>
<td style="width: 55%; height: 1-px; text-align: left;" rowspan="1">	
By connecting to the physical robot controller, you can retrieve the robot’s data and control GERTY.</td>
</tr>
</tbody>
</table>
</div>

## Output

* **ControllerInfo** : Allows you to check the connected robot data. 
* **SystemID** :  Outputs data such as the axis values and tool data of the virtual or real robot to assist with the simulation.
