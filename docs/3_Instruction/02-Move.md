---
title: Move
parent: 3. Instruction
layout: default
nav_order: 2
permalink: /ko/02-Move/
translation_link: /en/02-Move/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# Move

## Description

* TCP 움직임을 위해, RobTarget의 데이터를 받아 Move Instruction을 정의하는 컴포넌트이다. 각 타겟들의 움직임은 Type, Speed, Zone 옵션들로 설정할 수 있다.

<p align="center">  <img src="/assets/images/Move_2.png" align="center" width="25%"></p>

## Input

* **RobTargets** : RobTargets의 데이터를 받는다.

### Built-in Param | Move

* **MoveJ** : Move Joint로, 로봇이 해석한 최적의 자세인 정기구학으로 읽어 들어 Target Plane에 도달한다.
* **MoveL** : Move Leaner로, 사용자가 정의한 로봇의 자세에서 Target Plane을 역기구학으로 읽어 들어 최단거리를 찾아 도달한다.
* **Speed** : RobTarget에 도달하는 속도(Velocity)를 mm/s단위로 설정한다.
* **Zone** : Target Point를 중심으로 한 반경 범위로, 다음 Target Point로 이동시, zone값에 비례한 Radius크기 만큼 Filet하여 움직임을 제어한다. Fine을 정확하게 해당 포인트를 지나쳐야 하되, 로봇의 등속 움직임에 영향을 미칠 수 있다.

<p align="center"> 
<video src="/assets/images/Move_gif_confirm-min_SHL.mp4" width="576px" height="324px" autoplay=1 muted=1 loop=1 align="center"></video>
</p>

## Output

* **Instructions** : 입력된 Input에 따라 정의된 Move Instructions을 출력한다.
