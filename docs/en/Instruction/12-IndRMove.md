---
title: IndRMove
parent: Instruction
layout: default
nav_order: 2
permalink: /en/12-IndRMove/
translation_link: /ko/12-IndRMove/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# IndRMove

## Description

* `IndRMove` is a component that moves the positioner to a new joint angle based on the selected option and redefines its posture accordingly.
Supported options include `Short`, `Forward`, and `Backward`, each influencing the movement direction and angle resolution.
The final angle can also be redefined using a specified `ToRelDegree` value to guide the reset behavior.

<p align="center">  <img src="/assets/images/IndRMove_00.png" align="center" width="25%"></p>

## Input

* **MechUnit** : Specifies the name of the actual positioner robot. (Default is *STN1*)
* **AxisNum** : Specifies the index of the axis to be reset.

### Built-in Param | IndRMove

* **ToRelDegree** : Sets the target angle for resetting. The axis will be rotated and redefined to the nearest possible configuration relative to the current posture.
* **ResetType** : Determines how the angle is redefined based on the selected option. (Refer to the table for details)
* **RamSpeed** : Specifies the acceleration/deceleration speed (as a percentage) when moving toward the defined target angle.

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

* **Instructions** : Outputs an IndRMove instruction defined according to the specified input conditions.