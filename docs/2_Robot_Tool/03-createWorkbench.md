---
title: CreateWorkbench
parent: 2. Robot/Tool
layout: default
nav_order: 2
permalink: /ko/03-createWorkbench/
translation_link: /en/03-createWorkbench/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# CreateWorkbench

## Description

* Work Bench 모델링을 사용자 정의할 수 있는 컴포넌트이다.

<p align="center">  <img src="/assets/images/Workbench.png" align="center" width="25%"></p>

## Input

* **WorkBenchMesh[Mesh]** : workbench 모델링 메쉬를 받는다.
* **WorkBenchBasePl[Plane]** : 해당 workbench 모델링의 Base Plane을 잡는다.
* **WorkBenchFCPl[Plane]** : workbench Flange Center Plane을 잡는다.
* **Export [Boolean]** : 사용자는 해당 워크벤치를 저장할 수 있다.

<p align="center"> 
<video src="/assets/images/Workbench_Export.mp4" width="576px" height="230px" autoplay=1 muted=1 loop=1 align="center"></video><figcaption>Workbench Export</figcaption>
</p>

### Built-in Param : Basic Params

* **Display Colour** : 시뮬레이션 로봇의 색상을 선택한다.
* **Objs Colour** : Object의 색을 선정한다.

<br>

## Output

* **Workbench**: 사용자 정의된 Workbench 정보를 내보낸다.
