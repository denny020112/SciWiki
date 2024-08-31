---
aliases:
  - 자유도
category:
  - 물리학
related_concepts:
  - 고전역학
  - 물리
tags:
  - 물리
  - 고전역학
  - 통계학
  - 화학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 자유도 (Degrees of Freedom)
## 정의 및 개요

자유도 (Degrees of Freedom)란 어떤 계 내 에서의 운동을 설명하기 위해 필요한 변수의 개수이다. 주로 직선 운동 상태와 회전 운동 상태의 변수들을 모두 고려하여 산정한다.
어떤 물체의 운동에 대한 자유도는 구속 조건 혹은 구속력에 의해 줄어들 수 있다. 더 적은 자유도는 물체의 움직임을 더 쉽게 계산할 수 있도록 해준다. 

### 예시

아무것도 없는 텅 빈 공간에 펜이 하나 있다고 생각해보도록 하자. 이 펜은 직선방향으로 고려했을 때 상하, 좌우, 전후, 즉 x, y, z 세 축으로 움직일 수 있을 것이다. 그러므로 직선 운동의 자유도는 3이다. 
이번에는 이 펜이 회전할 수 있는 방식을 생각해보도록 하자. 펜이 풍차처럼 펜의 길이에 수직인 회전축을 기준으로 회전할 수 있을 것이다. 다른방향으로 수직인 회전축을 추가로 생각해볼 수도 있을 것이다. 그리고 드릴과 같이 이 펜의 길이 자체를 회전축으로 가지는 회전 또한 가능할 것이다.  그러면 회전 운동에서의 자유도는 3이다.
그러면 이때의 총 자유도는 3+3, 즉 6이 된다.

## 통계학에서의 자유도

자유도는 통계적 추정에서 자유롭게 변할 수 있는 값의 수를 나타낸다. 
표본의 크기가 n일 때, 자유도는 일반적으로 n-1이다. 이는 표본 평균을 계산할 때 n개의 값 중 n-1개만 자유롭게 변할 수 있기 때문이다.

### 왜 n-1인가?

1. 제약 조건: 표본 평균이 고정되면, n번째 값은 나머지 n-1개 값에 의해 결정된다.

2. 수학적 설명: 
   - 표본의 각 값을 x_i라 하고, 표본 평균을 x̄라 할 때:
   - $\sum_{i=1}^n (x_i - \bar{x}) = 0$ 이어야 한다.
   - 따라서 n-1개의 값이 정해지면, 마지막 값은 자동으로 결정된다.

3. 불편추정량: n-1로 나누면 모분산의 불편추정량이 된다.

### 예시

5개의 숫자가 있고 평균이 10이라면:
- 처음 4개 숫자는 자유롭게 선택할 수 있다.
- 하지만 5번째 숫자는 평균이 10이 되도록 자동으로 결정된다. 즉, 자유도가 없는 숫자가 된다.


