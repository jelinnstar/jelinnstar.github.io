---
title: WaitTime
parent: Instruction
layout: default
nav_order: 2
permalink: /en/10-WaitTime/
translation_link: /ko/10-WaitTime/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# WaitTime

## Description

* This component defines the WaitTime Instruction, which allows setting a pause time in seconds during the execution of a program to momentarily stop the robot's movement.

<p align="center">  <img src="/assets/images/WaitTime.png" align="center" width="25%"></p>

## Input

* **Time [Double]**: Enter a numeric value (Double) in seconds.

### Built-in Param | WaitTime

* **In Position [Boolean]** : Delays after reaching the specified Target Point position.
* **Time(sec.)** : Set the delay time in seconds.

## Output

* **Instructions** : Outputs WaitTime Data to be placed in the Instructions.
