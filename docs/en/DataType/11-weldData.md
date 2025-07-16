---
title: WeldData
parent: DataType
layout: default
nav_order: 2
permalink: /en/11-weldData/
translation_link: /ko/11-weldData/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# WeldData

## Description

* *welddata* is a component used to control welding operations during the *weld phase*, when the arc is active.

<p align="center">  <img src="/assets/images/WeldData.PNG" align="center" width="25%"></p>

## Input

* **Weld Name** : Sets the variable name for the WeldData.
* **Weld ArcData** : Connects the Weld ArcData to the component.
* **WeaveData** : Connects the WeaveData to the component.

### Built-in Param | Weld Phase Params

* **Weld Speed(mm/s)** : The original weld speed during the weld phase.(original weld speed)

<br>

## Output

* **WeldData** : Outputs the configured option values as a WeldData object.
* **Code** : Converts the configured WeldData into a code representation, allowing users to preview the actual settings in advance.
