---
title: SetDO
parent: 3. Instruction
layout: default
nav_order: 2
permalink: /ko/08-SetDO/
translation_link: /en/08-SetDO/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# SetDO

## Description

* ABB Controller의 Digital output 신호를 제어할 수 있는 SetDO Instruction을 정의하는 컴포넌트이다. Flex pendant내 신호데이터의 이름(변수명)과 해당 DigitalOutput 값을 할당한다.

<p align="center">  <img src="/assets/images/SetDO.png" align="center" width="25%"></p>

## Input

* **Signal [Text]** : Controller에 설정된 Digital Output 신호와 동일한 변수명을 입력한다.
* **Value [Text/Number]** : 0 또는 1의 디지털 신호를 입력한다.

## Output

* **Instructions** : Instructions에 넣을 SetDO로 출력한다.