---
title: GetUSBIDs
parent: 8. Setup
layout: default
nav_order: 2
permalink: /ko/02_GetUSBIDs/
translation_link: /en/02_GetUSBIDs/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# GetUSBIDs

## Description

* GetUSBIDs는 사용자의 로컬 PC에 귀속된 MAC주소가 아닌 USB에 귀속된 MAC주소를 사용하여 라이센스를 발급한다.
* PC에 귀속된 라이센스와 달리 PC가 달라져도 USB를 연결하여 GERTY를 사용할 수 있다.

<p align="center">  <img src="/assets/images/GetUSBIDs.png" align="center" width="25%"></p>

## Input
### Built-in Param | GERTY License:user information

* **Refresh** : 해당 라이센스 상태를 업데이트 한다.

## Output

* **USBInfo** : PC에 연결된 USB의 정보를 가져온다. 
* **USBID** : USB의 고유 주소를 불러온다. 