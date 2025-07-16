---
title: FileImportAndExport
parent: 8. Setup
layout: default
nav_order: 2
permalink: /ko/00_FileImportAndExport/
translation_link: /en/00_FileImportAndExport/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# FileImportAndExport

## Description

* FileImport&Export 는 GERTY 라이센스, 툴, 워크벤치와 같은 파일을 불러오거나 내보내어 추가, 백업해 사용할 수 있는 컴포넌트이다.
* 크게 불러오기(Import)와 내보내기(Export) 기능을 선택적 사용함에 따라 파일 주소나, 파일 컨텐츠들을 다수 선택할 수 있다.

<p align="center">  <img src="/assets/images/FileImportAndExport.png" align="center" width="25%"></p>

## Input

* **FileDir** : 불러오기 또는 내보내기 할  파일 디렉토리 주소 또는 파일(들)을 입력/선택 한다.
* **Generate** : 버튼을 연결하여, 상태를 업데이트 한다.

### Built-in Param : Actions |  type

* **Transfer** : 불러오기 또는 내보내기의 상태를 입력/선택한다.
* **File** : 불러오기 또는 내보내기할 데이터를 타입을 선택한다.


