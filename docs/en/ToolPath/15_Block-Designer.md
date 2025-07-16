---
title: Block Designer
parent: ToolPath
layout: default
nav_order: 2
permalink: /en/15_Block-Designer/
translation_link: /ko/15_Block-Designer/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# Block Designer

## Description

* Component for generating Target Planes used in Toolpaths for modeling Block Walls, utilizing relevant data from Unit Block and Wall-shaped surface modeling to plan the modeling of Block Walls and arrange individual Blocks.

<p align="center"><img src="/assets/images/BlockDesigner.png" align="center" width="25%"></p>

## Input

* **Base Plane [Plane]** : Sets the reference plane for the Unit Block, which determines the orientation direction for the Gripper TCP later on. 
* **Unit Block [Box]** : Inputs the Unit Block modeling to be used in Box format.
* **Wall [Brep]** : Inputs the modeling of the shape where the bricks will be stacked.

<p align="center"><img src="/assets/images/blockdesigner-1.png" align="center" width="80%"></p>

### Built-in Param | BlockDesign

* **Divide by Distance [Boolean]** : 
> **False (default)** : In this mode, the configured Horizontal Spacing serves as the minimum spacing condition, placing bricks at points that divide each layer.
> **True**: In this mode, the Horizontal Spacing for all layers is directly applied as set, without additional division.

* **Horizontal Spacing** : Adjusts the horizontal distance between adjacent blocks.
* **Vertical Spacing**: Adjusts the vertical distance between adjacent layers.

## Output

* **Block Count [int]**: Outputs the total number of blocks required for the stacking.
* **Target Planes [Plane]**: Outputs the target planes that define the positions and orientations of the placed blocks.
* **Block Wall [Mesh]**: Outputs the mesh collection of the generated block wall.
* **Layers [Curve]**: Outputs the curve collection representing the base layers of the stacked blocks.