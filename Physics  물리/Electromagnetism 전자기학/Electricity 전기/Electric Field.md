---
aliases:
  - Electric field
  - 전계
category:
  - 전기전자
  - 물리학
related_concepts:
  - 전하
  - 전위
  - 가우스 법칙
  - 쿨롱의 법칙
tags:
  - 전자기학
  - 벡터장
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
# 전기장 (Electric Field)

## 정의

전기장은 공간상의 각 지점에서 단위 전하가 받는 전기력을 나타내는 벡터장이다. 전하의 존재나 시간에 따라 변하는 자기장에 의해 발생한다.

$$ \mathbf{E} = \frac{\mathbf{F}}{q} $$

여기서:
- $\mathbf{E}$: 전기장 (N/C 또는 V/m)
- $\mathbf{F}$: 전기력 (N)
- $q$: 전하량 (C)

## 물리적 특성

1. 벡터량: 크기와 방향을 가진다.
2. 중첩의 원리: 여러 전하에 의한 전기장은 각 전하에 의한 전기장의 벡터합이다.
3. 연속성: 공간상에서 연속적으로 변화한다 (특이점 제외).

### 점전하에 의한 전기장

점전하 $Q$로부터 거리 $r$ 떨어진 지점에서의 전기장:

$$ \mathbf{E} = \frac{1}{4\pi\epsilon_0} \frac{q}{r^2} \hat{r} $$

여기서:
- $\epsilon_0$: 진공의 유전율
- $\hat{r}$: 점전하로부터 바깥쪽을 향하는 단위벡터

### 전기장의 시각화
![[visualisation of efield.png|500]]

1. 전기력선: 전기장의 방향과 세기를 나타내는 곡선. 양전하에서 나와 음전하로 양하는 화살표로써 표현된다.
2. 등전위면: 전위가 같은 점들을 연결한 면

### 전위와의 관계

전기장은 전위의 음의 기울기이다:

$$ \mathbf{E} = -\nabla V $$

여기서 $V$는 전위이다.

나블라의 사용이 익숙하지 않은 경우를 위해 나블라를 사용하지 않는 방식으로 정리하기 위해 퍼텐셜 에너지의 정의에서부터 천천히 확인해보도록 하자.
$$U=-\int_{R}^{P}\vec{F}\cdot d\vec{r}$$
전기장의 정의($q\vec{E}=\vec{F}$)를 이용해 사용하며 식을 변형해보면 다음과 같다:
$$U=-\int_{R}^{P}\vec{F}\cdot d\vec{r}=-q\int_{R}^{P}\vec{E}\cdot d\vec{r}$$
이때 전기 퍼텐셜의 정의($qV=U$)를 적용하면
$$U=-q\int_{R}^{P}\vec{E}\cdot d\vec{r}\ \ \longrightarrow V=-\int_{R}^{P}\vec{E}\cdot d\vec{r}$$
즉, 전기장은 퍼텐셜의 음의 기울기라는 것이 적분의 형태로 표현됨을 알 수 있다.

### 전기장의 에너지 밀도

단위 부피당 저장된 에너지:

$$ u = \frac{1}{2} \varepsilon_0 E^2 $$

### 가우스 법칙
*[[Gauss's Law|가우스 법칙]] 문서 참고*

전기장과 전하 분포의 관계를 나타내는 법칙:

$$ \oint \mathbf{E} \cdot d\mathbf{A} = \frac{Q_{enc}}{\varepsilon_0} $$

여기서 $Q_{enc}$는 폐곡면 내부의 총 전하량이다.


## 관련 개념

- [[Electromagnetic Field|전자기장]]
- [[Coulomb's Law|쿨롱의 법칙]]
- [[Gauss's Law|가우스의 법칙]]
- [[Electric Potential|전위]]

## 참고문헌

1. Griffiths, D.J. (2017). Introduction to Electrodynamics (4th ed.). Cambridge University Press.
2. Purcell, E.M., & Morin, D.J. (2013). Electricity and Magnetism (3rd ed.). Cambridge University Press.
3. Feynman, R.P., Leighton, R.B., & Sands, M. (2011). The Feynman Lectures on Physics, Vol. II: Mainly Electromagnetism and Matter. Basic Books.