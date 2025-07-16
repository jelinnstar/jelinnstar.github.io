---
title: TriggIOs
parent: DataType
layout: default
nav_order: 2
permalink: /en/06-TriggIOs/
translation_link: /ko/06-TriggIOs/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# TriggIOs

## Description

* The TriggIOs component is used to replace specific IO signals with user-defined values based on its internal IOData configuration.
triggios is used to define conditions and actions for setting a digital output signal, a group of digital output signals, or an analog output signal at a fixed position along the robot’s movement path.

<p align="center">  <img src="/assets/images/TriggIOs.png" align="center" width="25%"></p>

## Input

* **Name [String]** : Specifies the name of the signal. (e.g., ExtrudeON, ExtrudeOFF)
* **IOs** : Connects the signal to a unique I/O identifier defined by the user.

<p align="center">  <img src="/assets/images/TriggIOstemplate.png" align="center" width="80%"></p>

<br>

## Output

* **TriggIOs** : Outputs the configured signal data as `TriggIOs` values, which are then connected to the `TriggIOMove` component.
