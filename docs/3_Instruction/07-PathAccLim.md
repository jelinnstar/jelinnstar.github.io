---
title: PathAccLim
parent: 3. Instruction
layout: default
nav_order: 2
permalink: /ko/07-PathAccLim/
translation_link: /en/07-PathAccLim/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# PathAccLim

## Description

* TCP의 이동속도를 줄여주는 PathAccLim Instruction을 정의하는 컴포넌트이다. Target Point로의 위치까지 도달하기 위한, 로봇의 가속도(AccLim) 혹은 감속도(DecelLim)를 제한한다.

<p align="center">  <img src="/assets/images/PathAccLim_1.png" align="center" width="25%"></p>

<br>

## Input
* **RobTargets** : RobTargets의 데이터를 받는다.

### Built-in Param | Basic Params

* **AccLim [Boolean]** : 가속 활성화 여부를 묻는다. 기본값은 False.
* **DecelLim [Boolean]** : 감속 활성화 여부를 묻는다. 기본값은 False.
* **AccMax(m/s2)** : 최대 가속도 값을 입력한다.
* **DecelMax(m/s2)** : 최대 감속도 값을 입력한다.

## Output

* **Instructions** : 입력된 Input에 따라 정의된 PathAccLim Instructions을 출력한다.

# Example

다음은 PathAccLim 컴포넌트를 사용하였을 때 마주할 수 있는 예시입니다.

`Example 1`

- PathAccLim TRUE \AccMax := 4, TRUE \DecelMax := 4; TCP acceleration and TCP deceleration are limited to 4 m/s2. 

`Example 2`

- PathAccLim FALSE, FALSE; The TCP acceleration and deceleration is reset to maximum (default).