---
title: WorkbenchImporter
parent: Robot/Tool
layout: default
nav_order: 2
permalink: /en/05-workbenchImporter/
translation_link: /ko/05-workbenchImporter/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# WorkbenchImporter

## Description

* This component is for loading tool information extracted through the Workbench Exporter. It includes official BAT tools and can also load user-defined tool information. 
The Workbench Importer component has two modes: "Get Workbench Data" and "Get Workbench Input Data." 
In the "Get Workbench Data" mode, it provides complete Workbench information, which can be used as a substitute for the Workbench component. In the "Get Workbench Input Data" mode, it provides editable information that can be combined with the Workbench component to utilize customized data.

<p align="center">  <img src="/assets/images/WorkbenchImporter.png" align="center" width="50%"></p>


# Built-in Param | Basic Params

* **Model** : GERTY retrieves the selected tool information by checking the list of tool information stored in the repository.

# Output

## Get Tool Data - Mode

* **Tool Data** : The entered tool name (Name), tool modeling (Mesh), flange (Base Plane), TCP, Mass, Centroid, and Inertia values are exported as Tool Data.

## Get Tool Data Input - Mode

* **Name [String]** : Exports the entered tool name.
* **Tool Geometry [Mesh]** : Exports the entered tool modeling (Mesh).
* **Base Plane [Plane]** : Exports the tool base plane that attaches to the robot's sixth flange.
* **TCP [Plane]** : Exports the Tool Center Plane (TCP) value of the tool.
* **Mass [Double]** : Exports the mass information of the tool.
* **Centeroid [Generic Number]** : Exports the tool's center of mass value (e.g., in the form of 0,0,0).
* **Inertia [Generic Number]** : Exports the tool's moment of inertia value (e.g., in the form of 0,0,0).

<p align="center"> 
<video src="/assets/images/WorkbenchImporter_gif.mp4" width="576px" height="324px" autoplay=1 muted=1 loop=1 align="center">
</video>
</p>
