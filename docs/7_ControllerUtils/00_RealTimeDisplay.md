---
title: RealTimeDisplay
parent: 7. Controller Utils
layout: default
nav_order: 2
permalink: /ko/00_RealTimeDisplay/
translation_link: /en/00_RealTimeDisplay/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# RealTimeDisplay

## Description

* RealTimeDisplay는 실제 혹은 가상의 로봇 ID와 연결하여, 연결된 로봇의 움직임을 GERTY 시뮬레이션 움직임과 동기화 하여 관찰 할 수 있는 컴포넌트이다.

<p align="center">  <img src="/assets/images/realtimedisplay.png" align="center" width="40%"></p>

## Input

* **GERTY Robot**: 로봇 컴포넌트 데이터를 입력받는다.
* **SystemID** : 로봇 컨트롤러 데이터를 입력받는다.

## Built-in Param | CurrentTCP

* **Types**: 실제 로봇에 장작된 정보를 읽어 온다. 기본 값은 Tool
* **Options**: 출력할 로봇의 정보 옵션을 선택할 수 있다.

## Output

* **Robot Angle** : 로봇 각 축의 각도 값을 가져와 출력한다.
* **External Angle** : 부가축의 각도 값을 가져와 출력한다.
* **CurrentPos**: 로봇의 현재 자세를 출력한다.

## How To Use

* 다음은 RealTimeDisplay 컴포넌트 사용시 마주할 수 있는 예시이다.

<p align="center">  <img src="/assets/images/RealTimeDisplay_00-768x249.png" align="center" width="90%"></p>

<p align="center"> 
<video src="/assets/images/IMG_0556-2.mp4" width="576px" height="324px" autoplay=1 muted=1 loop=1 align="center">
</video>
</p>

