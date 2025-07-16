---
title: OverhangRangeColor
parent: 6. Utils
layout: default
nav_order: 2
permalink: /ko/06_OverhangRangeColor/
translation_link: /en/06_OverhangRangeColor/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# OverhangRangeColor

## Description

* OverhangeRangeColor는 작업물 출력 범위를 색상으로 표시하는 컴포넌트이다. 작업물의 기울기의 최대값이 45도를 넘어설 경우 회색 색상으로 표시되며, 작업물의 기울어짐 정도는 0도부터 45도까지 10등분되어 각 영역은 푸른계열에서 붉은 계열로 표시된다

<p align="center">  <img src="/assets/images/overhangrangecolor.png" align="center" width="25%"></p>

## Input

* **Mesh** : 메쉬(Mesh) 값을 입력받는다.
* **BasePlane** : 메쉬(Mesh)의 기준 평면을 입력한다. 기본값은 WorldXY  

## Output

* **Mesh** : 기울기 영역 별 색상의 메쉬값을 출력한다.
* **AngleData** : 기준평면에 적용된 메쉬의 각도값을 출력한다. 

## How To Use

* 작업 메쉬(Mesh)를 입력한 후 색상 스펙트럼으로 오버행(Overhang) 정도를 파악한다.

<p align="center">  <img src="/assets/images/overhagerangecolor_01-768x310.png" align="center" width="80%"></p>
<p align="center">  <img src="/assets/images/overhagerangecolor_02-768x284.png" align="center" width="80%"></p>

