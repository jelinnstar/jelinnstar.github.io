---
title: SurfaceFrame
parent: Utils
layout: default
nav_order: 2
permalink: /en/04_SurfaceFrame/
translation_link: /ko/04_SurfaceFrame/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# SurfaceFrame

## Description

* A component that takes an input surface and UV parameters to output the tangent plane at a specific location on the surface, with that location as the origin.

<p align="center">  <img src="/assets/images/surfaceframe.png" align="center" width="25%"></p>

## Input

* **Surface [Surface/Item]** :  Input the surface for which to compute the tangent plane.

### Built-in Param

* **U-Param [double/Item]** : Sets the U-direction parameter of the surface.
* **V-Param [double/Item]** : Sets the V-direction parameter of the surface.

## Output

* **BasePlane [Plane/item]** : Outputs the defined tangent plane based on the input conditions.
