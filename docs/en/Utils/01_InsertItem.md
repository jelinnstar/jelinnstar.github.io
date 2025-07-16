---
title: InsertItem
parent: Utils
layout: default
nav_order: 2
permalink: /en/01_InsertItem/
translation_link: /ko/01_InsertItem/
nav_exclude: true

---

<!-- [English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple } -->
[한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple }

{:toc}
# InsertItem

## Description

* Inserts an item or item collection into each branch of the input DataTree.
<p align="center">  <img src="/assets/images/insertTree.png" align="center" width="25%"></p>

## Input

* **Tree [Generic/DataTree]** :  Input the DataTree where items or item collections will be inserted.
* **Items [Generic/List]** : Input the items or item collections to be inserted.
* **indices [int/List]** : Input the indices within each branch where items or item collections will be inserted.

## Output

* **Tree [Generic/DataTree]** : Outputs the generated DataTree based on the input conditions.

## How To Use

* If the indices values corresponding to the positions where items or item indices will be inserted exceed the insertable index range within the branch, they will wrap around and be applied accordingly.

<p align="center">  <img src="/assets/images/Insert_Items_Exam-768x587.png" align="center" width="72%"></p>