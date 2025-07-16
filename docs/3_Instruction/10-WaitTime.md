---
title: WaitTime
parent: 3. Instruction
layout: default
nav_order: 2
permalink: /ko/10-WaitTime/
translation_link: /en/10-WaitTime/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# WaitTime

## Description

* 프로그램 실행 중 로봇의 동작을 잠시동안 멈추는 시간을 초 단위로 설정할 수 있는 WaitTime Instruction을 정의하는 컴포넌트이다.

<p align="center">  <img src="/assets/images/WaitTime.png" align="center" width="25%"></p>

## Input

* **Time [Double]**: 지연할 초단위를 숫자형식(Double)의 값으로 입력한다.

### Built-in Param | WaitTime

* **In Position [Boolean]** : 해당 Target Point 위치에 도달 후 지연한다.

## Output

* **Instructions** : Instructions에 넣을 WaitTime Data로 출력합니다