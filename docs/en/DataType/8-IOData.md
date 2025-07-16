---
title: IOData
parent: DataType
layout: default
nav_order: 2
permalink: /en/08-IOData/
translation_link: /ko/08-IOData/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# IOData

## Description

* It is a component that can define IO Data (Input/Output Data), i.e., signal data.

<p align="center">  <img src="/assets/images/IOData.png" align="center" width="25%"></p>


## Input

* **Signal [Text]** : Enter the variable name of the signal data.
* **Value [double]** : Specify the data value of the signal data.


### Built-in Param | Single Arc​

* **Used [Boolean]**: Check whether the signal is used. (Default: True)
* **Start [Boolean]**: Set the start point of the signal. (Default: false = End point)
* **Distance(mm)** : Define the signal of the device in mm from the StartPoint/EndPoint.
* **Equip Lag(sec.)** : Define the signal of the device in seconds from the StartPoint/EndPoint.

<figure>
	<a href="https://b-at.kr/wp-content/uploads/2023/05/IOData-768x250.png"><img src="https://b-at.kr/wp-content/uploads/2023/05/IOData-768x250.png"></a>
</figure>

<br>

## Output

* **IO Data** : Outputs the defined IO Data.

<figure>
	<a href="https://b-at.kr/wp-content/uploads/2024/07/0_flexpendant_signal_02.png"><img src="https://b-at.kr/wp-content/uploads/2024/07/0_flexpendant_signal_02.png"></a>
</figure>