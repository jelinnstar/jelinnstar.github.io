---
title: IndReset
parent: Instruction
layout: default
nav_order: 2
permalink: /en/11-IndReset/
translation_link: /ko/11-IndReset/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# IndReset

## Description

* `IndReset` is a component that recalculates and reassigns the positioner's joint angles to the nearest feasible configuration based on the selected optimization mode.
Supported modes include `Short`, `Forward`, and `Backward`, each providing a different strategy for minimizing angular displacement.

<p align="center">  <img src="/assets/images/IndReset_00.png" align="center" width="25%"></p>

## Input

* **MechUnit** : Specifies the name of the actual positioner robot. (Default is *STN1*)
* **AxisNum** : Specifies the index of the axis to be reset.

### Built-in Param | IndReset

* **RefDegree** : Defines the target angle value for resetting. The positioner’s current posture will be redefined to the nearest possible configuration relative to this angle.
* **ResetType** : Determines the angle reset strategy based on the selected option. (Refer to the table for details)

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

* **Instructions** : Outputs a IndReset instruction defined based on the given input conditions.
