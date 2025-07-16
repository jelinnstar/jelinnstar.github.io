---
title: BuildUp WAAM
parent: ToolPath
layout: default
nav_order: 2
permalink: /en/10_BuildUp-WAAM/
translation_link: /ko/10_BuildUp-WAAM/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# BuildUp WAAM

## Description

* Analyzes layered data to assist in creating WAAM ToolPaths.

<p align="center">  <img src="/assets/images/BuildupWAAM.png" align="center" width="25%"></p>

## Input

* **Deposition ToolPaths [DepositionToolPath / List]**: Receives DepositionToolPath data.
* **Is Bottommost [Boolean]**: Checks whether the WAAM deposition toolpaths start from the bottommost layer.

## Output

* **1st Shell Layers**: Extracts the first deposition layer.
* **1st Infill Layers**: Extracts the first infill layer.
* **Other Shell Layers**: Extracts the remaining deposition layers.
* **Other Infill Layers**: Extracts the remaining infill layers.