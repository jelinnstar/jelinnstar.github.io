---
title: AccSet
parent: 3. Instruction
layout: default
nav_order: 2
permalink: /ko/06-AccSet/
translation_link: /en/06-AccSet/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# AccSet

## Description

* Robot의 가속도를 제한하는 AccSet Instruction을 정의하는 컴포넌트이다.

<p align="center">  <img src="/assets/images/AccSet.png" align="center" width="25%"></p>

<br>

## Built-in Param | AccSet

* **Acceleration(%) [double]**: 동작의 최대 가(감)속도를 백분율로 제한한다.
* **Ramp(%) [double]** : 가(감)속도의 증가율을 제한한다.
* **FinePointRamp(%) [double]** : Fine Point에서 감속의 증가율을 추가적으로 제한한다. Fine Point에서 감속의 증가율은 Ramp * FinePointRamp으로 적용.

<p align="center">  <img src="https://b-at.kr/wp-content/uploads/2023/05/AccSet_1-1.png" align="center" width="72%"></p>

<br>

## Output

* **Instructions** : 입력된 Input에 따라 정의된 AccSet Instructions을 출력합니다
