---
title: SlicerFill
parent: 5. ToolPath
layout: default
nav_order: 2
permalink: /ko/11_SlicerFill/
translation_link: /en/11_SlicerFill/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# SlicerFill

## Description

* 적층 모델링의 내부 Shell을 채우는 툴패스를 생성하는 컴포넌트이다.

<p align="center">  <img src="/assets/images/SlicerFill.png" align="center" width="25%"></p>

## Input

* **GertyShellData [DataTree]**: 모델링을 적층 Shell Layer로 변환한 GERTYShellData를 입력한다.

### Built-in Param | Pattern Params

* **Int-infill Pattern** : Internal infill 툴패스의 채움 패턴을 정의한다. Zigzag, Rectangle, Triangle의 옵션을 선택한다. 기본 값은 Rectangle이다.
* **Ext-infill Pattern** :  Zigzag, Rectangle, Triangle 3가지의 채움 패턴을 정의한다. 기본 값은 Rectangle이다.

### Built-in Param | Slicing Params

* **Top Layer Count** : 윗 채움 레이어 개수를 정한다.
* **Bottom Layer Count** : 아래 채움 레이어 개수를 정한다.
* **Gap** : 외곽선와 채움 사이의 간격을 설정한다.(mm)
* **Int Infill Amount** : 속채움 양을 설정한다.

## Output

* **Deposition ToolPaths** : 속 채움 적층 툴 패스를 내보낸다.
* **Infill Polylines** : 속 채움 적층 툴패스 커브를 내보낸다.