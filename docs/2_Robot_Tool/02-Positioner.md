---
title: Positioner
parent: 2. Robot/Tool
layout: default
nav_order: 2
permalink: /ko/02-Positioner/
translation_link: /en/02-Positioner/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# Positioner

## Description

* ABB Positioner 기종 모델링을 사용자 정의할 수 있는 컴포넌트이다.

<p align="center">  <img src="/assets/images/Positioner.png" align="center" width="25%"></p>

## Input

* **Name [Text]** : Positioner 고유이름을 설정할 수 있다. 설정하지 않을 경우, 기본값으로 STN1으로 출력된다.
* **PositionerFCPL [Plane]**: Positioner Flange Center Plane의 약자로, 포지셔너 플랜지의 센터 플래인을 넣을 수 있다.
* **WorkBench [WorkBench Data]** : Positioner의 workbench 모델링을 넣을 수 있다.

### Built-in Param : Preview Params​

* **Model** : 포지셔너 모델을 지정한다.
* **Positioner Colour** : 포지셔너 모델의 색을 재정의한다.

### Built-in Param : Vector Params​

* **Enable Arm** : 포지셔너의 자세를 고정시킬 수 있다. 기본설정은 포지셔너 암 고정이 해제 되어있다.
* **Approaching Dir.** : 포지셔너에 접근하는 경로의 방향을 재정의한한다.
* **TCP Dir.** : 포지셔너에 접근하는 TCP의 방향을 재정의 재정의한한다.
<br>

## Output

* **GERTY Positioner** : 사용자 정의 된 포지셔너의 정보를 내보낸다.
* **Arm** : 로봇 암 현재 자세의 좌표값을 내보낸다.
* **Plate** :  로봇 작업대의 현재 Plane의 좌표값을 내보낸다.
* **ConnectPl** :  로봇 작업대와 포지셔너가 연결된 좌표 평면을 출력한다.

<p align="center"> 
<video src="/assets/images/Workbench_gif.mp4" width="576px" height="324px" autoplay=1 muted=1 loop=1 align="center">
</video>
</p>
