---
title: SurfaceFrame
parent: 6. Utils
layout: default
nav_order: 2
permalink: /ko/04_SurfaceFrame/
translation_link: /en/04_SurfaceFrame/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# SurfaceFrame

## Description

* 입력된 Surface와 UV파라미터 값을 통해, Surface위의 특정 위치를 원점으로 하고, 해당 지점에서 접평면(Tangent Plane)을 출력하는 컴포넌트. 

<p align="center">  <img src="/assets/images/surfaceframe.png" align="center" width="25%"></p>

## Input

* **Surface [Surface/Item]** : 접평면을 구할 Surface를 입력한다.

### Built-in Param

* **U-Param [double/Item]** : Surface의 U방향 파라미터를 설정한다.
* **V-Param [double/Item]** : Surface의 V방향 파라미터를 설정한다.

## Output

* **BasePlane [Plane / item]** : 입력한 조건에 따라, 정의된 접평면(Tangent Plane)을 출력한다. 

