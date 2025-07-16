---
title: GetMachineIDs
parent: Setup
layout: default
nav_order: 2
permalink: /en/01_GetMachineIDs/
translation_link: /ko/01_GetMachineIDs/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# GetMachineIDs

## Description

* This is a component for extracting the MAC address of the PC where GERTY will be installed and used. Currently, the GERTY license has two dependency methods: MAC address and USB ID. 
* Users can fill out the provided form with their MAC address and send it to contact@b-at.kr via the link within the component.

<p align="center">  <img src="/assets/images/GetMachineIDs.png" align="center" width="32%"></p>

## Input
### Built-in Param | GERTY License:Send MACAddress

* **Trial Request Page** : A link to the website for filling out the license form.

## Output

* **MACAddress** : Outputs the user’s unique MAC address value.

<p align="center"><img src="/assets/images/GetmachineIDs_00.png" align="center" width="65%"></p>