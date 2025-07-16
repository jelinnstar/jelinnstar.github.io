---
title: WorkbenchImporter
parent: 2. Robot/Tool
layout: default
nav_order: 2
permalink: /ko/05-workbenchImporter/
translation_link: /en/05-workbenchImporter/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# WorkbenchImporter

## Description

* Workbench Exporter를 통해 추출한 툴 정보를 불러오는 컴포넌트이다. BAT 공식 툴을 포함하고 있으며, 사용자가 정의한 툴 정보 또한 불러올 수 있다.
* Workbench Importer 컴포넌트는 “Get Workbench Data” 모드와 “Get Workbench Input Data ” 모드가 있다.
* 전자의 경우 완전한 워크벤치 정보값으로, Workbench컴포넌트를 대신해 사용할 수 있다. 후자의 경우 수정할 수 있는 정보값으로 Workbench 컴포넌트와 결합하여 사용자화 된 데이터로 사용할 수 있다.

<p align="center">  <img src="/assets/images/WorkbenchImporter.png" align="center" width="52%"></p>


### Built-in Param | Basic Params

* **Model** : GERTY 저장소에 있는 툴 정보 리스트를 확인하여 선택한 툴 정보를 불러온다.

## Output

### Workbench Data Common - Mode

* **Name [String]** : 입력한 툴 이름을 내보낸다.
* **Workbench Mesh [Mesh]** : 입력한 툴 모델링(Mesh)을 내보낸다.
* **Top Plane [Plane]** : 로봇 6번 플랜지에 장착 되는 툴 바닥면 Plane을 내보낸다.
* **Bottom Plane [Plane]** : 툴의 Tool Center Plane 값을 내보낸다.


### Workbench Data Detail - Mode

* **Tool Data** : 입력된 툴 이름(Name), 툴 모델링(Mesh), 플랜지(Base Plane), TCP, Mass, Centeroid, Inerta값을 Tool Data로 내보낸다.

<p align="center"> 
<video src="/assets/images/WorkbenchImporter_gif.mp4" width="576px" height="324px" autoplay=1 muted=1 loop=1 align="center">
</video>
</p>

