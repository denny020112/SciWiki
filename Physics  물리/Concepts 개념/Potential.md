---
aliases:
  - 포텐셜
  - 위치 에너지
category:
  - 물리학
  - 역학
  - 전자기학
related_concepts:
  - 에너지
  - 보존력
  - 스칼라장
tags:
  - 에너지
  - 역학
  - 전자기학
  - 물리
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 퍼텐셜 (Potential)

## 정의

퍼텐셜은 물리학에서 공간의 각 점에 할당된 스칼라 양으로, **그 지점에서 단위 입자나 단위 전하가 가질 수 있는 에너지를 나타낸다**. 주로 역학과 전자기학에서 중요하게 다뤄진다. 

## 수학적 표현

퍼텐셜 $V$는 일반적으로 다음과 같이 표현된다:

$$ V = \frac{U}{q} $$

여기서 $U$는 퍼텐셜 에너지, $q$는 단위 입자의 질량이나 전하량이다.


## 물리적 특징
퍼텐셜은 보존력 장에서만 정의되며, 주로 퍼텐셜의 절대적 총량 혹은 값 보다는 두 지점에서의 퍼텐셜 차이를 더 중점적으로 해석하는 경우가 일반적이다. 
단 여기서는 스칼라 퍼텐셜만 다루지만 벡터 퍼텐셜이라는 별개의 개념 또한 존재한다

### 퍼텐셜과 힘

퍼텐셜의 음의 기울기가 힘을 나타낸다:

$$ \vec{F} = -\nabla V $$

이는 보존력 장에서 일반적으로 성립한다.

### 유도

퍼텐셜은 일반적으로 힘으로부터 유도된다. 보존력 $\vec{F}$에 대해:

퍼텐셜 에너지 $U$의 변화:
   $$ dU = -\vec{F} \cdot d\vec{r} $$

두 점 a, b 사이의 퍼텐셜 차이:
   $$ V_b - V_a = -\int_a^b \vec{F} \cdot d\vec{r} $$

퍼텐셜의 정의:
   $$ V(\vec{r}) = -\int_{\infty}^{\vec{r}} \vec{F} \cdot d\vec{r'} $$

여기서 무한대를 기준점으로 사용했다.

### 퍼텐셜의 종류

#### 중력 퍼텐셜

중력장에서의 퍼텐셜 에너지를 질량으로 나눈 값:

$$ V_g = gh $$

여기서 $g$는 중력 가속도, $h$는 기준점으로부터의 높이다.

#### [[Electric Potential|전기 퍼텐셜]]

전기장에서의 퍼텐셜 에너지를 전하량으로 나눈 값:

$$ V_e = \frac{kq}{r} $$

여기서 $k$는 쿨롱 상수, $q$는 전하량, $r$은 전하로부터의 거리다.


## 연관 개념

1. 역학: 중력퍼텐셜, 탄성퍼텐셜 등
2. 전자기학: 전기퍼텐셜
3. 양자역학: 파동함수와 퍼텐셜 우물
4. 화학: 분자 간 상호작용

