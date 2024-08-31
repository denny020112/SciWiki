---
alias: [Q 테스트, Q-test] 
category: [통계학, 이상치 검출] 
related_concepts: [그럽스 테스트, Chauvenet's 테스트] 
tags: [이상치, 통계적 검정]
---
```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 딕슨 Q 테스트

## 정의

딕슨 Q 테스트는 작은 표본 크기의 데이터셋에서 이상치를 식별하기 위한 통계적 방법이다.

## 핵심 원리

1. 데이터를 정렬한다.
2. 의심되는 이상치와 가장 가까운 값의 차이를 전체 범위로 나눈다.
3. 계산된 Q 값을 임계값과 비교한다.

## 수학적 표현

Q 통계량은 다음과 같이 계산한다:

$$Q = \frac{|x_n - x_{n-1}|}{x_n - x_1}$$

여기서 $x_n$은 의심되는 이상치, $x_{n-1}$은 두 번째로 큰 값, $x_1$은 가장 작은 값이다.

### 예시

데이터셋: 10, 12, 14, 15, 16, 18, 25

Q 값 계산: (25 - 18) / (25 - 10) = 0.467

이 Q 값을 유의수준에 따른 임계값과 비교하여 이상치 여부를 판단한다.

## 장단점

장점:

- 작은 표본 크기에 적합하다
- 계산이 간단하다

단점:

- 큰 데이터셋에는 적합하지 않다
- 여러 이상치가 있을 경우 신뢰성이 떨어지며, 계산을 반복해야한다

## 관련 개념

- 그럽스 테스트
- Chauvenet's 테스트