---
title: WeldData
parent: 1. DataType
layout: default
nav_order: 2
permalink: /ko/11-weldData/
translation_link: /en/11-weldData/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# WeldData

## Description

* welddata는 아크가 형성되어 있는 용접 단계(weld phase) 동안 용접 동작을 제어하는 데 사용되는 컴포넌트이다.

<p align="center">  <img src="/assets/images/WeldData.PNG" align="center" width="25%"></p>

## Input

* **Weld Name** : WeldData 변수명을 설정한다.
* **Weld ArcData** : Weld ArcData를 연결한다.
* **WeaveData** : WeaveData를 연결한다.

### Built-in Param | Weld Phase Params

* **Weld Speed(mm/s)** : 속도를 설정한다.

<br>

## Output

* **WeldData** : 설정한 옵션 값을을 WeldData 값으로 출력한다.
* **Code** : 설정한 WeldData를 코드로 전환한 데이터로, 사용자는 실제 설정값을 사전에 확인할 수 있다.
