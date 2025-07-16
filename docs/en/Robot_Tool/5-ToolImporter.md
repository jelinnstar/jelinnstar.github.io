---
title: ToolImporter
parent: DataType
layout: default
nav_order: 2
permalink: /en/05-ToolImporter/
translation_link: /ko/05-ToolImporter/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# ToolImporter

## Description

* The Tool Importer component has "Get Tool Data" mode and "Get Tool Data Input" mode. In the former, the complete tool information can be used as the Tool Data input value for the Robot component. In the latter, the incomplete tool information can be used as the input value for the Tool Data component.

<p align="center">  <img src="/assets/images/toolimporter.png" align="center" width="50%"></p>

## Input
### Built-in Param | Basic Params​

* **Model** : Checks the tool information list in the GERTY repository and loads the selected tool information.

## Output

* The ToolImporter component has two mode options: GET TOOL DATA and GET TOOL DATA INPUT.
* In GET TOOL DATA mode, it can be directly connected to the robot component for use.
* In GET TOOL DATA INPUT mode, it can be used by modifying the tool status.

### 1. Get Tool Data​

* **Tool Data** : Exports the entered tool name (Name), tool modeling (Mesh), flange (Base Plane), TCP, Mass, Centroid, and Inertia values as Tool Data.

<p align="center">  <img src="/assets/images/2_ToolImporter_01.png" align="center" width="50%"></p>

### 2. Get Tool Data Input​

* **Name [String]** : Exports the entered tool name.
* **Tool Geometry [Mesh]** : Exports the entered tool modeling (Mesh).
* **Base Plane [Plane]** : Exports the tool base plane that is mounted on the robot's 6th flange.
* **TCP [Plane]** : Exports the Tool Center Point (TCP) value of the tool.
* **Mass [Double]** : Exports the mass information of the tool.
* **Centeroid [Generic Number]** : Exports the center of mass value of the tool (e.g., in the form of 0,0,0).
* **Inertia [Generic Number]** : Exports the moment of inertia value of the tool (e.g., in the form of 0,0,0).

<p align="center">  <img src="/assets/images/2_ToolImporter_02.png" align="center" width="90%"></p>
