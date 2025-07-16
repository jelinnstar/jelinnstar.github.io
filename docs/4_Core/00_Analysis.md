---
title: Analysis
parent: 4. Core
layout: default
nav_order: 2
permalink: /ko/00_Analysis/
translation_link: /en/00_Analysis/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# Analysis

## Description

* Analysis는 Core Solver에서 출력한 로봇의 에러 자세 및 인덱스 값을 분석하여 출력하는 컴포넌트이다. 사용자는 분석된 로봇의 에러 위치를 확인할 수 있다.

<p align="center">  <img src="/assets/images/Analysis.png" align="center" width="25%"></p>

## Input

* **GERTY Solver** : GERTY Solver 값을 연결한다.
<p align="center">  <img src="/assets/images/Analysis_template.png" align="center" width="80%"></p>

## Output

* **RobAx Angle** : 로봇 축과 각도 값을 출력한다.
* **Error Idx** : 로봇 에러 인덱스 값을 출력한다.
* **Error Report** : 에러 요인에 대한 정보를 출력한다.
<p align="center">  <img src="/assets/images/ErrorReport_00.png" align="center" width="80%"></p>