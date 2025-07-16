---
title: ScanToolData
parent: 7. Controller Utils
layout: default
nav_order: 2
permalink: /ko/03_ScanToolData/
translation_link: /en/03_ScanToolData/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# ScanToolData

## Description

* ScanToolData는 가상 혹은 실제 로봇의 현재 툴 데이터 정보 추출을 돕는 컴포넌트이다.

<p align="center">  <img src="/assets/images/ScanToolData.png" align="center" width="25%"></p>

## Input

* **SystemID** : 현재 컨트롤러에 연결된 로봇의 ID를 입력한다.

## Output

* **ToolName** : 현재 컨트롤러에 연결된 로봇의 툴 이름을 출력한다. 
* **TCP** : 현재 컨트롤러에 연결된 로봇의 TCP 데이터를 출력한다. 
* **Mass** : 현재 컨트롤러에 연결된 로봇의 툴 무게 데이터를 출력한다. 
* **Centroid** : 현재 컨트롤러에 연결된 로봇의 툴 Centroid 값을 출력한다. 
* **Inertia** : 현재 컨트롤러에 연결된 로봇의 툴 Inertia 값을 출력한다.

## How To Use
* ScanABBController로 현재 로봇 ID를 읽어와 ScanToolData에 연결하여 사용한다. 해당 로봇의 툴 데이터들을 추출하여 정교한 시뮬레이션을 돕는다.
<p align="center">  <img src="/assets/images/RealTimeDisplay_01-768x341 (1).png" align="center" width="90%"></p>
