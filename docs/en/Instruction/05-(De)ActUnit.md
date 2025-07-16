---
title: (De)ActUnit
parent: Instruction
layout: default
nav_order: 2
permalink: /en/05-(De)ActUnit/
translation_link: /ko/05-(De)ActUnit/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# (De)ActUnit

## Description

* (De)ActUnit is an instruction component that defines the activation (Activate) status of a robot unit. 
A robot unit refers to the individual control of two or more robots or additional axis equipment within a single controller.

<p align="center">  <img src="/assets/images/(De)ActUnit.png" align="center" width="25%"></p>

<br>

## Input

* **MechUnit [Text]**: Enter the name of the robot or additional axis device defined in the system. Default value: STN1

### Built-in Param | AccSet

* **Activate [Boolean]** : If True is entered, the ActUnit instruction is defined. If False is entered, the DeActUnit instruction is defined. (Default is True.)

<p align="center">  <img src="/assets/images/deactUnit_6.gif" align="center" width="72%"></p>

<br>

## Output

* **Instructions** : Outputs the defined (De)ActUnit Instruction.
