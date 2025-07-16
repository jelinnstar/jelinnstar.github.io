---
title: IndRMove
parent: 3. Instruction
layout: default
nav_order: 2
permalink: /ko/12-IndRMove/
translation_link: /en/12-IndRMove/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# IndRMove

## Description

* IndRMove는 포지셔너의 현재 자세를 설정한 옵션에 따라 해당 값으로 각도값으로 이동하여 재정의하는 컴포넌트이다.
옵션값은 Short, Forward, Bacward 가 있으며 ToRelDegree 설정 값에 따라 재정의 할 수도 있다.

<p align="center">  <img src="/assets/images/IndRMove_00.png" align="center" width="25%"></p>

## Input

* **MechUnit** : 실제 포지셔너 로봇의 이름을 입력한다.(기본값은 STN1) 
* **AxisNum** : 리셋할 축의 번호를 입력한다.

### Built-in Param | IndRMove

* **ToRelDegree** : 리셋할 각도 값을 설정하여 현재 자세에서 가장 가까운 값으로 회전, 재정의한다.
* **ResetType** : 옵션의 값에 따라 각도 값을 재정의 한다.(표 참고)
* **RamSpeed** : 설정한 각도값으로 이동하는 증감시의 가속도 속도값을을 설정한다.(%)

<p align="center">
<table style="border-collapse: collapse: width: 51 %; height: 150x;">
  <thead style="background-color: #F2F2F2; font-weight: bold; text-align: center;">
    <tr>
      <th style="width: 10%; height: 15px; text-align: center; font-weight: bolder;">ResetType</th>
      <td><strong>Description</strong></td>
    </tr>
  </thead>
  <tbody>   
    <tr>
      <th style="width: 25%; height: 15px; text-align: center; font-weight: bolder;">Short</th>
      <td style="width: 25%; height: 15px;">가장 짧은 각도 값으로 현재 축 각도 값 재정의.</td>
    </tr>
    <tr>  
      <th style="width: 25%; height: 15px; text-align: center; font-weight: bolder;">Fwd</th>
      <td style="width: 25%; height: 15px;">현재 축 각도 값을 360도로 나눈 나머지 각도 값 기준으로 재정의, i.e., <code>Angle % 360</code>.</td>
    </tr>
    <tr>
      <th style="width: 25%; height: 15px; text-align: center; font-weight: bolder;">Bwd</th>
      <td style="width: 25%; height: 15px;">현재 축 각도 값을 360도로 나눈 나머지 각도값을 360도에서 뺸 값을을 기준으로 재정의<code>360° - (Angle % 360)</code>.</td>
    </tr>
  </tbody>
</table>
</p>

## Output

* **Instructions** : 입력된 조건에 따라 정의된 IndRMove Instruction을 출력한다.