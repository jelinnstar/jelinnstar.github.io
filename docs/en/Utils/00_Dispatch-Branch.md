---
title: Dispatch Branch
parent: Utils
layout: default
nav_order: 2
permalink: /en/00_Dispatch-Branch/
translation_link: /ko/00_Dispatch-Branch/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# Dispatch Branch

## Description

* A component that splits the branches of an input DataTree into two DataTrees according to a pattern. Regardless of the format of individual paths in the input DataTree, the paths are separated by matching their sequence number with the pattern.

<p align="center">  <img src="/assets/images/dispatchbranch.png" align="center" width="25%"></p>

## Input

* **Tree [Generic / DataTree]** : Input the DataTree to be split according to the pattern.
* **Pattern [Bool / List]** : Input the list of boolean values to use as the split pattern. Branches matching “True” in the pattern are split into Tree_A, while branches matching “False” are split into Tree_B. 
  * For example, if the pattern is { True, False }, the branches of the odd-numbered paths in the input DataTree are split into Tree_A, and the branches of the even-numbered paths are split into Tree_B.

## Output

* **Tree A [Generic / DataTree]** : Outputs the DataTree composed of branch data matching “True” in the pattern
* **Tree B [bool / List]** : Outputs the DataTree composed of branch data matching “False” in the pattern.

## How To Use

* Here is an example you might encounter when using the Fly-By Branch component.

<p align="center">  <img src="/assets/images/DispatchBranch_exam-768x376.png" align="center" width="72%"></p>