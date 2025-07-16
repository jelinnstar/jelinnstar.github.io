---
title: SimplePathRemapper
parent: 6. Utils
layout: default
nav_order: 2
permalink: /ko/02_SimplePathRemapper/
translation_link: /en/02_SimplePathRemapper/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# SimplePathRemapper

## Description

* 입력된 DataTree의 각 Branch에 Item또는 Item Collection을 삽입합니다.
<p align="center">  <img src="/assets/images/simplepathremapper.png" align="center" width="25%"></p>

## Input

* **Tree [Generic/DataTree]** : Item또는 Item Collection을 삽입할 DataTree를 입력합니다.

### Context Menu Options

* `Sequential Path` : DataTree의 Path를 “[0],[1],[2],…” 의 순차적인 Path로 재정의합니다.
* `Odd Numbered Path` : DataTree의 Path를 “[1],[3],[5],…” 의 홀수 구성된 Path로 재정의합니다.
* `Even Numbered Path` : DataTree의 Path를 “[0],[2],[4],…” 의 짝수 구성된 Path로 재정의합니다.

## Output

* **Tree [Generic/DataTree]** : 입력된 조건에 따라, 생성된 DataTree를 출력합니다. 

## How To Use

<p align="center">  <img src="/assets/images/SimplePathRemapper_exam-768x631.png" align="center" width="72%"></p>
