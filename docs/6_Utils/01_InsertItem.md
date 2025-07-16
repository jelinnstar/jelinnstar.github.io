---
title: InsertItem
parent: 6. Utils
layout: default
nav_order: 2
permalink: /ko/01_InsertItem/
translation_link: /en/01_InsertItem/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# InsertItem

## Description

* 입력된 DataTree의 각 Branch에 Item또는 Item Collection을 삽입합니다.

<p align="center">  <img src="/assets/images/insertTree.png" align="center" width="25%"></p>

## Input

* **Tree [Generic/DataTree]** : Item또는 Item Collection을 삽입할 DataTree를 입력합니다.
* **Items [Generic/List]** : 삽입할 Item 또는 Item Collection을 입력합니다.
* **indices [int/List]** : 각 Branch 내에 Item 또는 Item Collection을 삽입할 인덱스를 입력합니다.

## Output

* **Tree [Generic/DataTree]** : 입력된 조건에 따라, 생성된 DataTree를 출력합니다. 

## How To Use

* Item 또는 Item index를 삽입할 위치에 해당하는 indices 값이 branch 내부에 삽입가능한 index 범위를 넘으면, Wrapping 된 값으로 적용됩니다.

<p align="center">  <img src="/assets/images/Insert_Items_Exam-768x587.png" align="center" width="72%"></p>
