---
title: SimplePathRemapper
parent: Utils
layout: default
nav_order: 2
permalink: /en/02_SimplePathRemapper/
translation_link: /ko/02_SimplePathRemapper/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# SimplePathRemapper

## Description

* Redefine the DataTree path according to Sequential / Odd numbered / Even numbered options.

<p align="center">  <img src="/assets/images/simplepathremapper.png" align="center" width="25%"></p>

## Input

* **Tree [Generic/DataTree]** : Enter the DataTree for which the Path will be redefined.

### Context Menu Options

* `Sequential Path` : Redefines the DataTree path as sequential paths such as “[0], [1], [2], …
* `Odd Numbered Path` : Redefines the DataTree path as paths with odd numbers, such as “[1], [3], [5], …
* `Even Numbered Path` : Redefines the DataTree path as paths with even numbers, such as “[0], [2], [4], …

## Output

* **Tree [Generic/DataTree]** : Outputs a DataTree with new paths mapped according to the specified conditions.

## How To Use

<p align="center">  <img src="/assets/images/SimplePathRemapper_exam-768x631.png" align="center" width="72%"></p>