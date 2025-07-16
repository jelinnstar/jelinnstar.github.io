---
title: WeaveData
parent: DataType
layout: default
nav_order: 2
permalink: /en/10-weaveData/
translation_link: /ko/10-weaveData/
nav_exclude: true
---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# WeaveData

## Description

* weavedata is used to define all weaving operations performed during arc welding.

<p align="center"><img src="/assets/images/weavedata.png" align="center" width="25%"></p>

## Input

* **Name** : Sets the variable name for the WeaveData.

### Built-in Param | WeaveData

* **Shape** : Sets the welding pattern. Available options are: `None`, `ZigZag`, `V-Shaped`, `Triangular`, and `Circular`.
<p align="center"><img src="/assets/images/ArcShape.png" align="center" width="65%"></p>

* **Type**: Specifies the type of welding weave. Available options are `Geometric`, `Wrist`, `Rapid_1`, and `Rapid_2`.  
  - *Geometric*: Geometric weaving using all robot axes.  
  - *Wrist*: Wrist weaving using only the wrist joints.  
  - *Rapid_1*: Rapid weaving using axes 1, 2, and 3.  
  - *Rapid_2*: Rapid weaving using axes 4, 5, and 6.

* **Length(mm)** : The `weave_length` component is defined as the length of one weaving cycle during the weld phase for weaving types 0 and 1.
<p align="center"><img src="/assets/images/weave_length.PNG" align="center" width="72%"></p>

* **Width(mm)** : Width refers to the span of the weaving cycle and is used to define the amplitude of the weave.
<p align="center"><img src="/assets/images/weave_width.PNG" align="center" width="72%"></p>

* **Height(mm)** : Height refers to the lift height of the robot during weaving and is used to define the vertical displacement of the weave.
<p align="center"><img src="/assets/images/weave_height.PNG" align="center" width="72%"></p>

  - `Image Source: ABB Robotics Documentation (© ABB, 2004–2018)`
<br>

## Output

* **WeaveData**: Outputs the configured welding weave settings as a *WeaveData* object.  
* **Code**: Converts the configured weave data into a code representation, allowing users to preview the actual welding parameters in advance.


