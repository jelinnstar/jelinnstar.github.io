---
title: Installation
parent: GERTY
layout: default
lang: en
permalink: /en/1-installation/
translation_link: /ko/1-installation/
nav_exclude: true

---
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }
{:toc}

# Installation

## 1. PackageManager

In Rhino's `PackageManager`, search for `GERTY` and install the latest version.<br> 
Restart Rhino after installation.<br>
The trial license will be activated automatically and can be used for **15 days**.<br>

If `Automatically update packages when Rhino starts` is selected, the latest version of GERTY will always be used.

<figure>
	<a href="https://i.postimg.cc/hPqP5NGm/0-packagemanager-00.png"><img src="https://i.postimg.cc/hPqP5NGm/0-packagemanager-00.png"></a>
</figure>



## 2. GetMachineIDs

If the Trial License expires, you can subscribe to GERTY's paid service.<br> 
When purchasing a license, use the **GetMachineIDs** component to retrieve the unique MAC address data.<br> 
Copy the extracted data using **"Copy Data Only"**, which can be accessed by right-clicking on the panel.

<figure>
	<a href="https://i.postimg.cc/y6D9qVd0/Getmachine-IDs-00.png"><img src="https://i.postimg.cc/y6D9qVd0/Getmachine-IDs-00.png"></a>
</figure>

Paste the copied MAC address into the form on the page linked to the **Trial Request Page** button and submit it.<br> 
If the form is not visible, send an email to **contact@b-at.kr**.

<figure>
	<a href="https://i.postimg.cc/WbhgR9g7/1-MACAddress-01.png"><img src="https://i.postimg.cc/WbhgR9g7/1-MACAddress-01.png"></a>
</figure>



## 3. FileImportAndExport

User will receive the license via email.<br> 
Use the **FileImporterAndExporter** component to apply the license.<br> 
Right-click on the **FilePath** component, select **"Select one existing file"**, and link the license file.

<figure>
	<a href="https://i.postimg.cc/1XxtLHQv/2-license-Import-1.png"><img src="https://i.postimg.cc/1XxtLHQv/2-license-Import-1.png"></a>
</figure>


Use the **GERTYLicense** component to check your license information.<br> 
If **Available** is confirmed, the GERTY installation is complete.<br> 
For any other issues, contact **contact@b-at.kr**.


