---
title: PathAccLim
parent: Instruction
layout: default
nav_order: 2
permalink: /en/07-PathAccLim/
translation_link: /ko/07-PathAccLim/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# PathAccLim

## Description

* This component defines the PathAccLim Instruction, which reduces the TCP's movement speed. It limits the robot's acceleration (AccLim) or deceleration (DecelLim) to reach the Target Point position.

<p align="center">  <img src="/assets/images/PathAccLim_1.png" align="center" width="25%"></p>

## Input
* **RobTargets** : Receives data from RobTargets.

### Built-in Param | Basic Params

* **AccLim [Boolean]** : Asks whether acceleration is enabled. Default is False.  
* **DecelLim [Boolean]** : Asks whether deceleration is enabled. Default is False.  
* **AccMax(m/s2)** : Inputs the maximum acceleration value. 
* **DecelMax(m/s2)** : Inputs the maximum deceleration value.

## Output

* **Instructions** : Outputs the defined PathAccLim Instructions based on the entered Input.

## Example

Here is an example of using the PathAccLim component:

`Example 1`

- PathAccLim TRUE \AccMax := 4, TRUE \DecelMax := 4; TCP acceleration and TCP deceleration are limited to 4 m/s2. 

`Example 2`

- PathAccLim FALSE, FALSE; The TCP acceleration and deceleration is reset to maximum (default).