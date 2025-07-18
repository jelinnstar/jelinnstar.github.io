---
title: Analysis
parent: Core
layout: default
nav_order: 2
permalink: /en/00_Analysis/
translation_link: /ko/00_Analysis/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# Analysis

## Description

* Analysis is a component that analyzes and outputs the robot error postures and index values generated by the Core Solver.
It allows users to identify the locations where robot errors occur.

<p align="center">  <img src="/assets/images/Analysis.png" align="center" width="25%"></p>

## Input

* **GERTY Solver** : Connects the `GERTY Solver` values to the component.
<p align="center">  <img src="/assets/images/Analysis_template.png" align="center" width="80%"></p>

## Output

* **RobAx Angle**: Outputs the robot joint indices and corresponding angle values.  
* **Error Idx**: Outputs the index values where robot errors have occurred.  
* **Error Report**: Outputs detailed information regarding the causes of the errors.
<p align="center">  <img src="/assets/images/ErrorReport_00.png" align="center" width="80%"></p>
