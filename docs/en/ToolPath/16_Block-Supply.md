---
title: Block Supply
parent: ToolPath
layout: default
nav_order: 2
permalink: /en/16_Block-Supply/
translation_link: /ko/16_Block-Supply/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# Block Supply

## Description

* A component that models the unit block used in the planned block wall, models the supply block stack, and creates the target plane for picking up the block based on data such as the total number of blocks needed.

<p align="center"><img src="/assets/images/BlockSupply.png" align="center" width="25%"></p>

## Input

* **Base Plane [Plane]** :  Input the reference plane that defines the position and orientation of the generated block stack.
* **Unit Block [Box]** : Input the unit block model in the form of a box.
* **Spacing [Box]** :Input the array cell defining the spacing of the unit block’s box array.
* **Block Count [int]** : Input the total number of blocks to be used.

### Built-in Param | Basic Params

* **X Count** : Defines the number of blocks to array in the X direction.
* **Y Count** : Defines the number of blocks to array in the Y direction.
* **Z Count** : Defines the number of blocks to array in the Z direction.

## Output

* **Blocks [Mesh]** : Outputs the mesh collection of the supply block stack model.
* **Target Planes [Plane/List]** : Outputs the target planes located at the picking points of each block in the supply.