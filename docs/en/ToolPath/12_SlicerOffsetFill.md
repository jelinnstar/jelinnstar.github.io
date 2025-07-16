---
title: SlicerOffsetFill
parent: ToolPath
layout: default
nav_order: 2
permalink: /en/12_SlicerOffsetFill/
translation_link: /ko/12_SlicerOffsetFill/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# SlicerOffsetFill

## Description

* This is a component for generating toolpaths to fill the internal Shell of layered modeling. 
It determines the fill using an offset method of the outer curve shape.

<p align="center">  <img src="/assets/images/SlicerOffsetFill.png" align="center" width="25%"></p>

## Input

* **GertyShellData [DataTree]** : Input GERTYShellData, which has been converted into a layered Shell Layer for modeling.
* **Direction** : The fill direction can be adjusted to forward or reverse.

<p align="center"><img src="/assets/images/direction-1.png" align="center" width="70%"></p>

## Output

* **Infill ToolPaths** : Outputs the infill toolpaths.
* **Infill Polyines** : Outputs the infill layer as curve values.