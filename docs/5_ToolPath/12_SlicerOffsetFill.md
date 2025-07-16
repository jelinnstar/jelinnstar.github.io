---
title: SlicerOffsetFill
parent: 5. ToolPath
layout: default
nav_order: 2
permalink: /ko/12_SlicerOffsetFill/
translation_link: /en/12_SlicerOffsetFill/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# SlicerOffsetFill

## Description

* 적층 모델링의 내부 Shell을 채우는 툴패스를 생성하는 컴포넌트이다.
외곽 커브 형태의 옵셋(Offset)된 방식을 채택하여 채움을 결정한다.

<p align="center"><img src="/assets/images/SlicerOffsetFill.png" align="center" width="25%"></p>

## Input

* **GertyShellData [DataTree]** : 모델링을 적층 Shell Layer로 변환한 GERTYShellData를 입력한다.
* **Direction** : 채움 방향을 정방향/역방향으로 수정할 수 있다.

<p align="center"><img src="/assets/images/direction-1.png" align="center" width="70%"></p>

## Output

* **Infill ToolPaths** : 채움 툴패스(ToolPath)를 출력한다.
* **Infill Polyines** : 채움 레이어를 커브(Curve) 값으로 출력한다.