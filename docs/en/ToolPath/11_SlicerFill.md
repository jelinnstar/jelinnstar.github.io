---
title: SlicerFill
parent: ToolPath
layout: default
nav_order: 2
permalink: /en/11_SlicerFill/
translation_link: /ko/11_SlicerFill/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# SlicerFill

## Description

* A component that generates toolpaths to fill the internal shell of an additive modeling structure.

<p align="center">  <img src="/assets/images/SlicerFill.png" align="center" width="25%"></p>

## Input

* **GertyShellData [DataTree]**: Inputs GERTYShellData, which converts the modeling into additive Shell Layers.

### Built-in Param | Pattern Params

* **Int-infill Pattern** : Defines the internal infill toolpath pattern. Options include Zigzag, Rectangle, and Triangle. The default is Rectangle.
* **Ext-infill Pattern** :  Defines the external infill pattern with three options: Zigzag, Rectangle, and Triangle. The default is Rectangle.

### Built-in Param | Slicing Params

* **Top Layer Count**: Specifies the number of top infill layers.
* **Bottom Layer Count**: Specifies the number of bottom infill layers.
* **Gap**: Sets the gap between the outline and the infill (mm).
* **Int Infill Amount**: Sets the amount of internal infill.

## Output

* **Deposition ToolPaths**: Outputs the internal infill additive toolpaths.
* **Infill Polylines**: Outputs the infill additive toolpath curves.