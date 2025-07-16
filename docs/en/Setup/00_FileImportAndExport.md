---
title: FileImportAndExport
parent: Setup
layout: default
nav_order: 2
permalink: /en/00_FileImportAndExport/
translation_link: /ko/00_FileImportAndExport/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# FileImportAndExport

## Description

* FileImport&Export is a component that allows you to import or export files such as GERTY licenses, tools, and workbenches for additional use or backup. Depending on whether you choose the import or export function, you can select multiple file addresses or file contents.

<p align="center">  <img src="/assets/images/FileImportAndExport.png" align="center" width="25%"></p>

## Input

* **FileDir** : Enter/select the file directory address or files to import or export. 
* **Generate** : Connect the button to update the status.

### Built-in Param | Actions:type

* **Transfer** : Enter/select the status of the import or export. 
* **File** : Select the type of data to import or export.
