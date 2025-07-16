---
title: BuildUp WAAM
parent: 5. ToolPath
layout: default
nav_order: 2
permalink: /ko/10_BuildUp-WAAM/
translation_link: /en/10_BuildUp-WAAM/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# BuildUp WAAM

## Description

* 적층 데이터를 분석하여 WAAM 툴패스의 작성을 돕는 컴포넌트이다.

<p align="center"><img src="/assets/images/BuildupWAAM.png" align="center" width="25%"></p>

## Input

* **Deposition ToolPaths [DepositionToolPath/List]** : DepositionToolPath Data를 받는다.
* **Is Bottommost [Boolean]** : 바닥면부터 시작되는 WAAM 적층 툴패스 여부를 확인한다.

## Output

* **1st Shell Layers** : 첫 번째 적층 Layer를 추출한다.
* **1st Infill Layers** : 첫 번째 채움 Layer를 추출한다.
* **Other Shell Layers** : 다른 적층 Layer를 추출한다.
* **Other Infill Layers** : 다른 채움 Layer를 추출한다.