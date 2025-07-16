---
title: ToolPathPartition
parent: Utils
layout: default
nav_order: 2
permalink: /en/07_ToolPathPartition/
translation_link: /ko/07_ToolPathPartition/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# ToolPathPartition

## Description

* The ToolPathsPartition is a component that allows different conditions to be set for the start and end points. The length of the settings for the start and end points cannot exceed the total length of the layer. If the settings exceed this length, the values for each respective point will be reset and output as percentages.

<p align="center">  <img src="/assets/images/toolpathpartition.png" align="center" width="25%"></p>

## Input

* **TargetPlanes[Plane]** : Connects the major paths of the previous results’ TargetPlanes.

### Built-in Param | Partition

* **Start(mm)** : Determines the partition distance (mm) from the start point.  
* **End(mm)** : Determines the partition distance (mm) from the end point.  
* **Substitution(%)** : If the distance value settings exceed the actual length of the distance, the partition for the respective point can be set as a percentage.

<p align="center">  <img src="/assets/images/partitionSplit_00.png" align="center" width="92%"></p>

## Output

* **Targets** : Outputs the target planes divided by partitions.  
* **Index** : Outputs the indexes of the start and end points for the partitioned sections. 
* **Domain** : Outputs the domains of each layer.