---
aliases:
  - 키르히호프의 법칙
category:
  - 전기전자
  - 물리학
related_concepts:
  - 전하
  - 전위
  - 기전력
  - 전압
  - 전류
tags:
  - 전자기학
  - 물리
  - 전기회로
  - 전기
---
```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 키르히호프의 법칙 (Kirchhoff's Law)
## 정의
독일의 물리학자 구스타프 키르히호프(Gustav Kirchhoff)가 19세기에 회로의 전류와 전압에 대하여 정립한 법칙이다. 
## 설명
### 제 1 법칙
![[kirchhoff_current_law_final.png|400]]
키르히호프의 1 법칙, 혹은 키르히호프의 전류법칙 (Kirchhoff's Current Law; KCL).
$$\sum\limits_{k}I_{k}=0$$
회로 안에서 *어느 지점이건* 들어간 전류의 합과 나온 전류의 합은 동일하다. 통상적으로 들어가는 전류는 양수(+), 나가는 전류는 음수(-)로 간주하여 계산한다.
주로 회로의 마디(node)별로 혹은 분기(junction)별로 기준을 잡고 확인을 했을 시에 드나든 전류의 양을  비교하여 확인할 수 있다. 이러한 특징으로 인해 마디 법칙(node rule) 혹은 분기 법칙(junction rule)이라고도 지칭된다.
전류법칙의 원리는 회로의 전하는 보존된다는 점에 의한 것이다. 
#### 예시
### 제 2 법칙
![[kirchhoff_voltage_law.png|400]]
키르히호프의 2 법칙, 혹은 키르히호프의 전압법칙 (Kirchhoff's Voltage Law; KVL).
$$\sum\limits_{j}V_{source,\ j}=\sum\limits_{k}V_{device,\ k}$$
회로 안에서 닫힌 경로를 기준으로 볼 때, 닫힌 구간 안에서 전압 강하(voltage drop)의 합은 기전력(emf)의 합과 같다. 즉, 닫힌 구간 혹은 고리 (loop) 내에서 전체 전압과 전압 강하의 합은 0이라는 것이다. 고리를 기준으로 잡고 계산을 주로 하기에 고리 법칙 (loop rule)이라고도 지칭한다.
원리를 생각해보자면, 기전력을 받고 전하를 운반하는 입자가(주로 전자일 것이다) 회로의 요소을 지나며 일을 하고 제자리로 돌아온 후, 다시 기전력을 받아 동일한 일을 반복한다. 즉, 이는 전원이 해준 일 만큼 에너지가 회로에 전해진다는 것이다. 회로에 들어온 에너지와 나간 에너지는 동일해야한다는 것이고, 이는 곧 회로의 에너지 보존 법칙을 의미한다고 할 수 있다.

#### 예시