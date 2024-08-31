---
aliases:
  - 양자 상태함수
  - 슈뢰딩거 파동함수
  - 파동함수
category:
  - 양자역학
  - 양자화학
related_concepts:
  - 슈뢰딩거 방정식
  - 확률 밀도
  - 양자 중첩
tags:
  - 양자역학
  - 확률론
  - 화학
  - 물리
  - 양자화학
  - 물리화학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 파동함수 (Wave Function)

## 정의

파동함수($\psi,\Psi$)는 양자역학적 시스템의 상태를 완전히 기술하는 수학적 함수이다. 이는 시스템의 모든 가능한 측정 결과에 대한 확률 정보를 포함한다. 주로 상황과 조건에 알맞은 [[Schrödinger's Equation|슈뢰딩거 방정식]]의 해이다.

## 수학적 표현

일반적으로 파동함수는 복소함수이며, 공간과 시간의 함수로 표현된다:

$$\Psi = \Psi(\mathbf{r}, t)$$

여기서 $\mathbf{r}$은 위치 벡터, $t$는 시간이다.

## 물리적 의미

### 파동함수의 특성

#### 연속성 

파동함수와 그 일차 도함수는 모든 공간에서 연속이어야 한다 (특정 불연속점 제외).
#### 단일값

파동함수는 각 공간점과 시간에서 단일 값을 가져야 한다.
#### 유한성

파동함수는 모든 공간에서 유한한 값을 가져야 한다.

#### 규격화 가능성

파동함수는 규격화 가능해야 한다
##### 파동함수의 규격화

파동함수의 규격화는 규격화 상수 $N$을 도입하여 전체 확률이 1이 되도록 하는 과정이다:
 
$$\int_{-\infty}^{\infty} |\Psi|^2 d\tau = 1$$
$$\Psi_{normalized} = N\Psi$$

### 해석

#### 확률 해석 (보른 해석)

$|\Psi|^2$는 특정 위치에서 입자를 발견할 확률 밀도를 나타낸다.

$$P(\mathbf{r}) = |\Psi(\mathbf{r})|^2 d\tau$$

#### 중첩 원리

시스템은 여러 상태의 중첩으로 존재할 수 있으며, 이는 파동함수의 선형 결합으로 표현된다:

$$\Psi = c_1\Psi_1 + c_2\Psi_2 + ... = \sum_i c_i\Psi_i$$

#### 관측에 의한 붕괴

측정 시 파동함수는 고유상태 중 하나로 붕괴한다. 이는 코펜하겐 해석의 핵심이다.

## 예시

### 무한 우물 퍼텐셜

무한 포텐셜 우물[^1] 내 입자의 파동함수:

$$\Psi_n(x) = \sqrt{\frac{2}{L}}\sin(\frac{n\pi x}{L})$$

여기서 $L$은 상자의 길이, $n$은 양자수이다.

### 조화 진동자

1차원 조화 진동자의 기저 상태 파동함수:

$$\Psi_0(x) = (\frac{m\omega}{\pi\hbar})^{1/4} e^{-\frac{m\omega x^2}{2\hbar}}$$

여기서 $m$은 질량, $\omega$는 각진동수이다.


## 관련 개념

- [[Schrödinger's Equation|슈뢰딩거 방정식]]
- [[Quantum Superposition]]
- [[Probability Density]]
- [[Quantum Measurement]]

## 참고문헌

1. Griffiths, D. J. (2018). Introduction to Quantum Mechanics. Cambridge University Press.
2. Cohen-Tannoudji, C., Diu, B., & Laloë, F. (1977). Quantum Mechanics. Wiley.
3. Sakurai, J. J., & Napolitano, J. (2017). Modern Quantum Mechanics. Cambridge University Press.



[^1]: 상자 안의 입자 라고도 한다.