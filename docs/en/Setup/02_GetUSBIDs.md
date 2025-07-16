---
title: GetUSBIDs
parent: Setup
layout: default
nav_order: 2
permalink: /en/02_GetUSBIDs/
translation_link: /ko/02_GetUSBIDs/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# GetUSBIDs

## Description

* GetUSBIDs issues a license based on the MAC address associated with the USB device, rather than the MAC address of the user’s local PC. 
* Unlike licenses tied to a specific PC, this allows GERTY to be used on different PCs as long as the USB device is connected.

<p align="center">  <img src="/assets/images/GetUSBIDs.png" align="center" width="25%"></p>

## Input
### Built-in Param | GERTY License:user information

* **Refresh** : Updates the status of the license.

## Output

* **USBInfo** : Retrieves information about the USB devices connected to the PC.
* **USBID** : Fetches the unique identifier of the USB device.
