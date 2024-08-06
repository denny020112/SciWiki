---
aliases:
  - 스칼라곱
category:
  - 선형대수학
related_concepts:
  - 벡터외적
  - 벡터의 크기
  - 코사인법칙
tags:
  - 벡터
  - 선형대수학
  - 수학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 벡터의 내적

## 정의

두 벡터 $\mathbf{a}$ 와 $\mathbf{b}$ 의 내적(dot product)은 다음과 같이 정의된다:

$$\mathbf{a} \cdot \mathbf{b} = |\mathbf{a}||\mathbf{b}|\cos\theta$$

여기서 $\theta$ 는 두 벡터 사이의 각도다.

## 성질

1. 교환법칙: $\mathbf{a} \cdot \mathbf{b} = \mathbf{b} \cdot \mathbf{a}$
2. 분배법칙: $\mathbf{a} \cdot (\mathbf{b} + \mathbf{c}) = \mathbf{a} \cdot \mathbf{b} + \mathbf{a} \cdot \mathbf{c}$
3. 결합법칙: $(k\mathbf{a}) \cdot \mathbf{b} = k(\mathbf{a} \cdot \mathbf{b})$, 여기서 $k$는 스칼라다.

## 계산 방법

3차원 공간에서 $\mathbf{a} = (a_1, a_2, a_3)$ 와 $\mathbf{b} = (b_1, b_2, b_3)$ 일 때:

$$\mathbf{a} \cdot \mathbf{b} = a_1b_1 + a_2b_2 + a_3b_3$$

## 기하학적 의미

- 내적의 결과는 스칼라다.
- $\mathbf{a} \cdot \mathbf{b} = 0$ 이면 두 벡터는 서로 수직이다.
- $\mathbf{a} \cdot \mathbf{a} = |\mathbf{a}|^2$

## 응용

1. 벡터의 크기 계산
2. 두 벡터 사이의 각도 계산
3. 한 벡터를 다른 벡터에 투영
4. 물리학에서 일(work) 계산

## 예제

$\mathbf{a} = (1, 2, 3)$ 와 $\mathbf{b} = (4, 5, 6)$ 의 내적을 구하면:

$$\mathbf{a} \cdot \mathbf{b} = 1(4) + 2(5) + 3(6) = 4 + 10 + 18 = 32$$