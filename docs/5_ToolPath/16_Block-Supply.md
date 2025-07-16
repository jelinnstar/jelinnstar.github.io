---
title: Block Supply
parent: 5. ToolPath
layout: default
nav_order: 2
permalink: /ko/16_Block-Supply/
translation_link: /en/16_Block-Supply/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# Block Supply

## Description

* 계획된 Block Wall에 사용된 Unit Block 모델링, 필요한 Block의 총 개수 등의 데이터로부터, 공급부 Block 더미 모델링 및  Block을 집어 올리는 Target Plane을 생성하는 컴포넌트.


<p align="center"><img src="/assets/images/BlockSupply.png" align="center" width="25%"></p>

## Input

* **Base Plane [Plane]** : 생성되는 Block 더미의 위치와 방향을 정의하는 기준 평면을 입력한다.
* **Unit Block [Box]** : 사용할 Unit Block 모델링을 Box 형식으로 입력한다.
* **Spacing [Box]** : Unit Block의 BoxArray 간격을 정의하는, Array Cell을입력한다.
* **Block Count [int]** : 사용될 Block의 총 개수를 입력한다.

### Built-in Param | Basic Params

* **X Count** : X 방향으로 Array할 Block 개수를 정의한다.
* **Y Count** : Y 방향으로 Array할 Block 개수를 정의한다.
* **Z Count** : Z 방향으로 Array할 Block 개수를 정의한다.

## Output

* **Blocks [Mesh]** : 공급부 Block 더미 모델링의 Mesh Collection을 출력한다.
* **Target Planes [Plane/List]** : 공급부 각 Block을 집는 지점에 위치한 Target Plane을 출력한다.