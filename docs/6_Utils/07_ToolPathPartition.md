---
title: ToolPathPartition
parent: 6. Utils
layout: default
nav_order: 2
permalink: /ko/07_ToolPathPartition/
translation_link: /en/07_ToolPathPartition/
---

[English]({{ site.baseurl }}/en{{ page.url | remove_first: '/ko' }}){: .btn .btn-purple }
<!-- [한국어]({{ site.baseurl }}/ko{{ page.url | remove_first: '/en' }}){: .btn .btn-purple } -->

{:toc}
# ToolPathPartition

## Description

* ToolPathsPartition은 시작과 끝 지점으로부터 조건을 다르게 설정할 수 있는 컴포넌트이다. 시작과 끝 지점의 설정 길이는 해당 레이어의 전체 길이을 넘을 수 없으며, 만약 초과되어 설정할 경우 각 해당 지점의 설정값은 퍼센트지로 재 설정되어 출력된다.

<p align="center">  <img src="/assets/images/toolpathpartition.png" align="center" width="25%"></p>

## Input

* **TargetPlanes[Plane]** : 이전 결과값의 주요경로 TargetPalnes를 연결한다.

### Built-in Param | Partition

* **Start(mm)** : 시작 지점부터의 파티션 거리(mm)를 결정한다.
* **End(mm)** : 끝 지점부터의 파티션 거리(mm)를 결정한다.
* **Substitution(%)** : 거리값 설정이 실제 거리값의 길이를 초과할 경우, 해당 지점의 파티션은 퍼센트지로 설정할 수 있다.

<p align="center">  <img src="/assets/images/partitionSplit_00.png" align="center" width="92%"></p>

## Output

* **Targets** : 파티션으로 나눠진 타켓 플레인(Target Palne)을 출력
* **Index** : 파티션으로 분할된 시작과 끝 지점의 인덱스들을 출력
* **Domain** : 각 레이어들의 도메인을 출력

