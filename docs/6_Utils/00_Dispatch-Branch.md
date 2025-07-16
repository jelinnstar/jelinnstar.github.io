---
title: Dispatch Branch
parent: 6. Utils
layout: default
nav_order: 2
permalink: /ko/00_Dispatch-Branch/
translation_link: /en/00_Dispatch-Branch/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# Dispatch Branch

## Description

* 입력된 DataTree의 Branch를 Pattern에 따라 2개의 DataTree로 분리하는 컴포넌트. 입력되는 DataTree 개별 Path의 형식과는 관련이 없이, Path의 순번과 Pattern을 매칭하여 분리한다. 

<p align="center">  <img src="/assets/images/dispatchbranch.png" align="center" width="25%"></p>

## Input

* **Tree [Generic/DataTree]** : 패턴에 따라 분리할 DataTree를 입력한다.
* **Pattern [Boolean/List]** : 분리 패턴으로 사용할 bool값을 List형식으로 입력한다. Pattern의 “True”에 매칭되는 Branch는 Tree_A, “False” 에 매칭되는 Branch는 Tree_B로 분리된다. 
  - e.g., Pattern = { True, false } 입력한 경우, Input으로 입력된, DataTree의 홀수번째 Path의 Branch가 Tree A로, 짝수번째 Path의 Branch가 Tree B로 분리됨.

## Output

* **Tree A [Generic/DataTree]** : Pattern의 “True”에 매칭되는 Branch데이터로 구성된 데이터트리를 출력한다.
* **Tree B [Boolean/List]** : Pattern의 “False”에 매칭되는 Branch데이터로 구성된 데이터트리를 출력한다.

## How To Use

* 다음은 Fly-By Branch 컴포넌트를 사용하였을 때 마주할 수 있는 예시다.

<p align="center">  <img src="/assets/images/DispatchBranch_exam-768x376.png" align="center" width="72%"></p>