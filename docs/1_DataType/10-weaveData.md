---
title: WeaveData
parent: 1. DataType
layout: default
nav_order: 2
permalink: /ko/10-weaveData/
translation_link: /en/10-weaveData/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# WeaveData

## Description

* weavedata는 아크 용접 중 수행되는 모든 위빙 동작을 정의하는 데 사용된다. 위빙은 용접 이음부의 가열(heat) 및 용접(weld) 단계에서 사용할 수 있다.

<p align="center"><img src="/assets/images/weavedata.png" align="center" width="25%"></p>

## Input

* **Name** : WeaveData의 변수 이름을 설정한다.

### Built-in Param | WeaveData

* **Shape** : 용접 형상을 설정한다. 옵션 값은 `None`, `ZigZag`, `V-Shaped`, `Triangular`, `Circular`가 있다.
<p align="center"><img src="/assets/images/ArcShape.png" align="center" width="65%"></p>

* **Type** : 용접 위빙 타입을 설정한다. 옵션 값은 `Geometric`, `Wrist`, `Rapid_1`, `Rapid_1` 가 있다.
  - *Geometric*: 기하학적 위빙. 모든 축을 사용하여 위빙을 수행한다.
  - *Wrist*: 손목 위빙. 손목 관절을 사용하여 위빙을 수행한다.
  - *Rapid_1*: 빠른 위빙. 1, 2, 3축을 사용.
  - *Rapid_2*: 빠른 위빙. 4, 5, 6축을 사용.

* **Length(mm)** : weave_length 컴포넌트가 위빙 유형 0과 1에서 용접 단계 동안의 하나의 위빙 사이클 길이로 정의된다.
<p align="center"><img src="/assets/images/weave_length.PNG" align="center" width="72%"></p>

* **Width(mm)** : 폭은 위빙시 사이클의 너비를 의미하며, 해당 너비를 설정한다.
<p align="center"><img src="/assets/images/weave_width.PNG" align="center" width="72%"></p>

* **Height(mm)** : 높이는 위빙시 로봇이 들어올리는 높이로, 해당 높이를 설정한다.
<p align="center"><img src="/assets/images/weave_height.PNG" align="center" width="72%"></p>

  - `Image Source: ABB Robotics Documentation (© ABB, 2004–2018)`
<br>

## Output

* **WeaveData** : 설정한 용접 위빙 데이터를 WeaveData로 치환해 내보낸다.
* **Code** : 설정한 용접 위빙 데이터를 코드로 전환한 데이터로, 사용자는 실제 용접 값 설정을 사전에 확인할 수 있다.

