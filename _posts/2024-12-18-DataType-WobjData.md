---
title: "WobjData"
layout: single
header:
  teaser: "https://b-at.kr/wp-content/uploads/2024/07/04_WobjData.png"

collection: Datatype
entries_layout: grid
author_profile: true

categories:
  - DataType
sidebar:
  nav: "sidebar"
toc: true
toc_label: "Contents"
toc_icon: "cog"
toc_sticky: true

tags: 
  - GERTY
---
# Description

WobjData는 로봇의 내부 작업객체를 정의하는 컴포넌트이다.
내부 작업물의 위치를 WobjData로부터 사용자 정의(UserFrame)로 만들 수 있으며, 로봇의 기종 및 부가축에 맞춰 Fixed WobjData와 MovableData로 변경한다.

<figure>
	<a href="https://b-at.kr/wp-content/uploads/2024/07/04_WobjData.png"><img src="https://b-at.kr/wp-content/uploads/2024/07/04_WobjData.png"></a>
</figure>


# Input

* **Name [Text]** : UserFrame의 변수명을 입력한다.
* **UserFrame [Plane]** : Base Plane을 설정한다.

## Built-in Param : Preview Params​

* **Used [Boolean]**: 해당 신호의 사용여부를 확인한다. (기본값 : True)
* **Start [Boolean]**: 해당 신호의 시작 포인트를 설정한다. (기본값 : false = End point)
* **Distance(mm)**: 장치의 신호를 StartPoint/EndPoint 지점으로부터 mm거리 단위로 정의할 수 있습니다.
* **Equip Lag(sec.)**: 장치의 신호를 StartPoint/EndPoint 지점으로부터 초 단위로 정의할 수 있습니다.

# Output

* **WobjData** : 정의된 WobjData를 출력한다.