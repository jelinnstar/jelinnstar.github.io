---
title: FlyByCustom
parent: 5. ToolPath
layout: default
nav_order: 2
permalink: /ko/02_FlyByCustom/
translation_link: /en/02_FlyByCustom/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# FlyByCustom

## Description

* 입력되는 로봇 TCP 주요 경로(Target Plane Input) DataTree의 각 Branch의 사이사이를 지나는, 새로운 이동경로를 생성하는 컴포넌트이다. FlyBy 컴포넌트는 기본적으로 입력된 주요경로 Branch[i]의 마지막 Plane과 인접한 주요경로 Branch[i+1]의 첫번째 Plane을 이용하여, 사용자가 입력한 거리만큼 떨어진 위치에, 새로운 FlyBy Target Plane들을 정의한다.

<p align="center">  <img src="/assets/images/FlyByCustom.png" align="center" width="25%"></p>

## Input

* **TargetPlanes [Plane/DataTree]**: FlyBy Targets을 적용하기 위해, TCP 주요 경로에 해당하는 Target Plane들을 입력한다.
* **Approaching Dir.** : 진입하는 이동경로의 방향을 사용자가 정의한다.
* **Leaving Dir.** : 진출하는 이동경로의 방향을 사용자가 정의한다.

### Built in param | Advanced Params

Advanced Param은 이동 경로의 프로파일을 결정하는 옵션입니다. 이동경로의 프로파일은, Builtin Parma : Basic 에서 사용자가 선택한 조건에 따라, 이동경로 처음과 마지막 Flyby Plane이 주요경로로부터 이격되는 방향 벡터를 Blend 하는 방식으로 결정된다.
  
  * **Continuity** : 선택하는 연속성 조건에 따라, 생성되는 FlyBy Plane들의 원점이 선형 또는 비선형 커브 위에 있도록 한다. 기본값 : Position(G0)
  
  `연속성 설명 참고 : Rhinoceros 도움말 – 연속성 설명 /| Rhino 3D 모델링 (mcneel.com)`

<div className="multi-headings" align="center">
  <table style="border-collapse: collapse: width: 51 %; height: 280px;">
    <thead>
      <tr>
        <th style="text-align: center;">Type</th>
        <th style="text-align: center;">Description</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th style="width: 45%; height: 20px; text-align: center;">Position(G0)</th>
        <td style="width: 45%; height: 20px;"> 이동경로의 첫번째와 마지막 Plane 원점의 위치만 연속성(G0)을 갖는 Blend Curve를 이동경로의 프로파일로 취합니다. </td>
      </tr>
      <tr>
        <th style="width: 45%; height: 20px; text-align: center;">Tangency(G1)</th>
        <td style="width: 45%; height: 20px;"> 이동경로의 첫번째와 마지막 Plane 원점의 위치와 해당 위치에서 이격 방향벡터와 같은 방향의 접선을 갖는, G1 연속성의 Blend Curve를 이동경로의 프로파일로 취합니다. </td>
      </tr>
      <tr>
        <th style="width: 45%; height: 20px; text-align: center;">Curvature(G2)</th>
        <td style="width: 45%; height: 20px;"> 이동경로의 첫번째와 마지막 Plane 원점의 위치와 해당 위치에서 이격 방향벡터와 같은 방향의 접선, 같은 곡률반지름을 갖는, G2 연속성의 Blend Curve를 이동경로의 프로파일로 취합니다.</td>
      </tr>
    </tbody>
  </table>
</div>

<p align="center"><img src="/assets/images/Untitled-1-2-768x223.png" align="center" width="80%"></p>
<p align="center"><img src="/assets/images/Untitled-2-1-768x457.png" align="center" width="80%"></p>
<p align="center"><img src="/assets/images/Untitled-3-1-768x418.png" align="center" width="80%"></p>

  * **Bulge Start** : (Tangency/Curvature 조건인 경우,) 0-1사이의 값을 입력하여, 연속성을 유지한 상태에서 이동경로 프로파일의 시작부분 형상을 편집한다.
  * **Bulge End** : (Tangency/Curvature 조건인 경우,)0-1사이의 값을 입력하여, 연속성을 유지한 상태에서 이동경로 프로파일의 끝부분 형상을 편집한다.

## Output

* **Fly-by Targets** : 입력된 조건에 따라, 생성된 이동경로를 DataTree 형태로 출력한다. 이때 FlyBy Targets Output은 주요경로에의 최초 진입/최후 진출에 해당하는 FlyBy Plane까지를 포함하기 때문에, Target Planes Input의 Branch 개수보다 1개 많은 Branch를 갖는다. 또, 이동경로 Instruction 할당 이후, 주요 경로에 대한 Instruction과 데이터 병합을 용이하게 하기 위해, [0]-[2]-[4]-… 로 시작하는 짝수의 Path를 갖는 DataTree가 된다.