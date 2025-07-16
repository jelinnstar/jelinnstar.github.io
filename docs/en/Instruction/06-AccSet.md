---
title: AccSet
parent: Instruction
layout: default
nav_order: 2
permalink: /en/06-AccSet/
translation_link: /ko/06-AccSet/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# AccSet

## Description

* This is a component that defines the AccSet Instruction to limit the acceleration of the robot.

<p align="center">  <img src="/assets/images/AccSet.png" align="center" width="25%"></p>

<br>

### Built-in Param | AccSet

* **Acceleration(%) [double]**: Limits the maximum acceleration (or deceleration) of the motion as a percentage.
* **Ramp(%) [double]** : Limits the rate of increase in acceleration (or deceleration).
* **FinePointRamp(%) [double]** : Further limits the rate of deceleration increase at Fine Points. The rate of deceleration increase at Fine Points is applied as Ramp * FinePointRamp.

<p align="center">  <img src="https://b-at.kr/wp-content/uploads/2023/05/AccSet_1-1.png" align="center" width="72%"></p>

<br>

## Output

* **Instructions** : Outputs the defined AccSet Instructions based on the entered Input.