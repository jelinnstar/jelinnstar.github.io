---
title: UVFinishing
parent: 5. ToolPath
layout: default
nav_order: 2
permalink: /ko/08_UVFinishing/
translation_link: /en/08_UVFinishing/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# UVFinishing

## Description

* 2차 밀링 단계의 컷팅 툴패스 컴포넌트이다. 아래의 그림처럼 길이가 다른 평행한 커브 사이의 Cutting Direction방향으로 같은 길이값으로 등분하여 출력한다.

<p align="center">  <img src="/assets/images/UV_Finishing.png" align="center" width="25%"></p>

## Input

* **Brep** : Brep 또는 Surface UV객체를 입력한다.
* **Reference Plane** : Tilting weight=0일 때, Target Orientation 기준 평면을 입력한다.

<p align="center"><img src="/assets/images/UVfinishing-768x238.png" align="center" width="80%"></p>

### Built-in Param | Basic Params

* **Cutting Direction [Boolean]** : U(False) / V(True) 방향  선택한다.
* **Stepover** : 수평방향으로 한번에 깎이는 정도로 기본값으로 엔드밀 직경의 절반 이하의 값을 입력한다.
작을수록 세밀한 Finishing을 할 수 있다. (Stepover <= 엔드밀 직경 * 1/2)
* **Tilting Weight** : Target Tilting 가중치로 0.0~1.0 사이의 값만 입력한다.  0에 가까울수록 BasePlane의 normal, 1에 가까울수록 Surface의 normal에 따라 Target Plane을 기울기이다.
* **Tolerance** : Toolpath 해상도이다.

## Output

* **Curve** : Finishing Layer의 커브를 출력한다.
* **Target Plane**: Plane 인덱스 값들을 DataTree로 출력한다.