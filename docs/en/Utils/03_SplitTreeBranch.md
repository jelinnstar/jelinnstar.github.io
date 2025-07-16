---
title: SplitTreeBranch
parent: Utils
layout: default
nav_order: 2
permalink: /en/03_SplitTreeBranch/
translation_link: /ko/03_SplitTreeBranch/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# SplitTreeBranch

## Description

* Splits the input DataTree into two DataTrees based on the sequence (index) of a specified path.

<p align="center">  <img src="/assets/images/splittreebranch.png" align="center" width="25%"></p>

## Input

* **Tree [Generic/DataTree]** : Input the DataTree to be split.
* **Index [Int/Item]** : Input the index that will serve as the splitting criterion. Branches up to and including the branch at the specified index path are stored in Tree A, while subsequent branches are stored in Tree B.

## Output

* **Tree A [Generic/DataTree]** : Outputs the separated front portion of the DataTree.
* **Tree B [Boolean/List]** : Outputs the separated rear portion of the DataTree.

## How To Use

Here is an example where the DataTree input splits Paths[1] up to Paths[2]~ the last Path into Tree A and Tree B, respectively.

<p align="center">  <img src="/assets/images/SplitTree_exam-768x374.png" align="center" width="72%"></p>