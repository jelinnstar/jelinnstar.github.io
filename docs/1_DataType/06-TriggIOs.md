---
title: TriggIOs
parent: 1. DataType
layout: default
nav_order: 2
permalink: /ko/06-TriggIOs/
translation_link: /en/6-TriggIOs/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# TriggIOs

## Description

* TriggIOs 컴포넌트는 고유의 IOData 값을 활용하여 사용자가 정의한 값으로 치환하여 내보내는 컴포넌트이다.
triggios는 로봇의 이동 경로상 고정된 위치에서 디지털 출력 신호, 디지털 출력 신호 그룹 또는 아날로그 출력 신호를 설정하기 위한 조건과 동작을 정의하는 데 사용된다.

<p align="center">  <img src="/assets/images/TriggIOs.png" align="center" width="25%"></p>

# Input

* **Name [String]** : 신호 이름을 작성한다. (e.g., `ExtrudeON` or `ExtrudeOFF`)
* **IOs** : 설정한 값의 고유 신호를 연결한다.

<p align="center">  <img src="/assets/images/TriggIOstemplate.png" align="center" width="80%"></p>

<br>

# Output

* **TriggIOs** : 설정한 신호 데이터를 `TriggIOs` 값으로 내보낸다. 이후 `TriggIOMove`에 연결한다.