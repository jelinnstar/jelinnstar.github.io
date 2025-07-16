---
title: WobjData
parent: 1. DataType
layout: default
nav_order: 2
permalink: /ko/03-WobjData/
translation_link: /en/3-WobjData/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# WobjData

## Description

* WobjData는 로봇의 내부 작업객체를 정의하는 컴포넌트이다. 내부 작업물의 위치를 WobjData로부터 사용자 정의(UserFrame)로 만들 수 있으며, 로봇의 기종 및 부가축에 맞춰 Fixed WobjData와 MovableData로 변경한다.

<p align="center">  <img src="/assets/images/04_WobjData.png" align="center" width="25%"></p>


## Input

* **Name [Text]** : UserFrame의 변수명을 입력한다.
* **UserFrame [Plane]** : Base Plane을 설정한다.

### Felxible Option

* **Fixed WobjData** : Target plane이 고정된 위치의 기준 평면으로로 재정의 된다.
* **Movable WobjData** : Target Plane이 이동성있는 위치의 기준 평면으로 재정의 된다.
<br>
<p align="center">  <img src="/assets/images/wobj_movable.png" align="center" width="45%"></p>

## Output

* **WobjData** : 정의된 WobjData를 출력한다.
