---
title: Sub Procedure
parent: 3. Instruction
layout: default
nav_order: 2
permalink: /ko/09-Sub-Procedure/
translation_link: /en/09-Sub-Procedure/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# Sub Procedure

### Description

* Sub Porcedures는 Main Procedures에 작성되는 신호 및 기타 모션이 반복적으로 수행될 경우, 해당 코드를 축약하여 호출 할 수 있도록 돕는다.

<p align="center">  <img src="/assets/images/SubPorcedure.png" align="center" width="25%"></p>

## Input

* **Name [Text]** : 호출 될 변수명을 입력한다.
* **Instructions** : 반복 수행하는 모션 코드를 입력한다.

## Output

* **Sub_Proc**. : 축약 된 코드를 Sub Procedure으로 출력한다.