---
title: TreeBranch
parent: Utils
layout: default
nav_order: 2
permalink: /en/05_TreeBranch/
translation_link: /ko/05_TreeBranch/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# TreeBranch

## Description

* Extracts specific branches from the input DataTree based on the sequence (index) of paths.

<p align="center">  <img src="/assets/images/treebranch.png" align="center" width="25%"></p>

## Input

* **Tree [Generic/DataTree]** : Input the DataTree from which specific branches will be extracted.
* **Index [Int/Item]** : Input the index of the path to be extracted.

## Output

* **Branch [Generic/DataTree]** : Outputs the branch at the specified path index.

## How To Use

As in the example below, branches are extracted based on the path index, and if the index value exceeds the total range of path indices, it wraps around.

<p align="center">  <img src="/assets/images/TreeBranch_exam-768x647.png" align="center" width="80%"></p>