---
title: SetDO
parent: Instruction
layout: default
nav_order: 2
permalink: /en/08-SetDO/
translation_link: /ko/08-SetDO/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# SetDO

## Description

* This component defines the SetDO Instruction, which controls the digital output signals of an ABB Controller. It assigns the variable name (signal data) and the corresponding DigitalOutput value from the Flex pendant.

<p align="center">  <img src="/assets/images/SetDO.png" align="center" width="25%"></p>

## Input

* **Signal [Text]** : Enter the variable name that corresponds to the Digital Output signal configured on the Controller.
* **Value [Text/Number]** : Enter a digital signal of 0 or 1.

## Output

* **Instructions** : Outputs SetDO to be placed in the Instructions.
