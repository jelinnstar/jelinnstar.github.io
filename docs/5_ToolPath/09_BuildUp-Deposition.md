---
title: BuildUp Deposition
parent: 5. ToolPath
layout: default
nav_order: 2
permalink: /ko/09_BuildUp-Deposition/
translation_link: /en/09_BuildUp-Deposition/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# BuildUp Deposition

## Description

* 적층 데이터를 분석하여 일반 적층 툴패스의 작성을 돕는 컴포넌트이다.

<p align="center">  <img src="/assets/images/BuildupDeposiiton.png" align="center" width="25%"></p>

## Input

* **Home Pos [Plane/Optional]** : 적층 시작 전 Home position에 해당하는 Plane을 입력한다. 기본 값으로 World XY을 받는다.
* **Deposition ToolPaths [DepositionToolPath/List]** : DepositionToolPath Data를 받는다.
* **Pre-Extrusion Curve [Curve/Optional]** : 노즐 클리닝을 위해, 미리 압출할 형상의  Curve 데이터를 받는다.
* **Is Bottommost [Boolean]** : 바닥면부터 시작되는 적층 툴패스 여부를 확인한다.

## Output

* **E-Start Planes** : 압출이 시작되는 주요경로의 첫번째 plane값을 출력한다.
* **Movement Planse** : 압출이 진행되는 주요경로 Plane값을 출력한다.
* **E-Stop Planes** : 압출이 멈추는 주요경로 위치의 plane값을 출력한다.
* **E-Stop idx** : E-Stop Plane의 index를 출력한다.