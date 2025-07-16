---
title: ArcMove
parent: Instruction
layout: default
nav_order: 2
permalink: /en/01-ArcMove/
translation_link: /ko/01-ArcMove/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# ArcMove

## Description

* The component used to control the robot's motion utilizes ArcData. Therefore, it must take ArcData as input.

<p align="center">  <img src="/assets/images/ArcMove.png" align="center" width="25%"></p>

## Input

* **RobTargets** : Inputs the RobTarget to which ArcMove will be applied.
* **SeamData** : Inputs the SeamData created from the DataType.
* **WeldData** : Inputs the WeldData created from the DataType.

### arc Move | Built-in Params

* **Type** : Selects the type of motion action. ArcL, ArcC.
* **Speed** : Controls the movement speed of the robot.
* **Zone** : Controls the accuracy of reaching the target point. The fine value acts as a stop position, overriding the robot's continuous motion control.

## Output

* **Instructions** : Outputs the defined ArcMove instructions based on the given inputs.