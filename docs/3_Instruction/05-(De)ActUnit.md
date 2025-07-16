---
title: (De)ActUnit
parent: 3. Instruction
layout: default
nav_order: 2
permalink: /ko/05-(De)ActUnit/
translation_link: /en/05-(De)ActUnit/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# (De)ActUnit

## Description

* (De)ActUnit은 로봇 개체(Unit)의 활성화(Activate) 여부를 정의하는 instruction 컴포넌트이다.
* 로봇 개체(Unit)는 2가지 이상의 로봇이나 부가축 장비를 하나의 컨트롤러에서 제어하는 경우, 각 장치의 단위를 의미한다.
<p align="center">  <img src="/assets/images/(De)ActUnit.png" align="center" width="25%"></p>

## Input

* **MechUnit [Text]**: 시스템에 정의된 로봇 또는 부가축 장치의 이름을 입력한다. 기본값: STN1

### Built-in Param | AccSet

* **Activate [Boolean]** : True가 입력된 경우, ActUnit 인스트럭션이 정의된다. False 가 입력된 경우, DeActUnit 인스트럭션이 정의된다. (기본값 True.)

<p align="center">  <img src="/assets/images/deactUnit_6.gif" align="center" width="72%"></p>

<br>

## Output

* **Instructions** : 정의된 (De)ActUnit Instruction을 출력한다.
