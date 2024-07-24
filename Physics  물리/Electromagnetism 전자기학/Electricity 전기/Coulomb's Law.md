---
aliases:
  - Coulomb's Law
  - 정전기력 법칙
category:
  - 물리학
  - 전자기학
related_concepts:
  - 전기력
  - 전하
  - 역제곱 법칙
tags:
  - 전자기학
  - 쿨롱
  - 물리
  - 전하
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 쿨롱의 법칙

## 개요

쿨롱의 법칙은 두 전하 사이에 작용하는 정전기력을 설명하는 물리 법칙이다. 1785년 프랑스의 물리학자 샤를-오귀스탱 드 쿨롱에 의해 발견되었다.

## 법칙

두 점전하 사이에 작용하는 정전기력의 크기는 두 전하의 곱에 비례하고, 그 거리의 제곱에 반비례한다.

### 수학적 표현

$$ F = k \frac{|q_1 q_2|}{r^2} =\frac{1}{4\pi \epsilon_{0} \epsilon_{r}} \frac{|q_1 q_2|}{r^2} $$

여기서:
- $F$는 정전기력의 크기
- $k$는 쿨롱 상수 ($k = 8.99 \times 10^9 \, \mathrm{N \cdot m^2/C^2}$)
	- $k=\frac{1}{4\pi \epsilon_{0} \epsilon_{r}}$으로, $\epsilon_{0}$은 유전율(permittivity), $\epsilon_{r}$은 비유전율(relative permittivity)이다[^1].
- $q_1$, $q_2$는 각 전하의 크기
- $r$은 두 전하 사이의 거리

### 벡터 형태

$$ \vec{F} = k \frac{q_1 q_2}{r^2} \hat{r} $$

여기서 $\hat{r}$은 한 전하에서 다른 전하를 향하는 단위 벡터이다.

## 주요 특징

1. 역제곱 법칙: $$\vec{F}\propto \frac{1}{r^2}$$거리의 제곱에 반비례한다.
2. 중첩의 원리: 여러 전하에 의한 힘은 각 전하에 의한 힘의 벡터 합이다.
3. 인력과 척력: 같은 부호의 전하는 척력, 다른 부호의 전하는 인력이 작용한다.

## 적용 예시

1. 원자 구조: 전자와 원자핵 사이의 상호작용
2. 정전기 현상: 머리카락이 빗에 달라붙는 현상
3. 번개: 구름과 지면 사이의 전하 이동

## 쿨롱 법칙의 중요성

1. 전자기학의 기초: 맥스웰 방정식의 기본이 된다.
2. 물질의 구조 이해: 원자와 분자의 결합을 설명하는 데 필수적이다.
3. 기술 응용: 정전기 스프레이, 복사기, 레이저 프린터 등에 활용된다.

## 한계점

1. 점전하 가정: 실제 전하 분포가 크기를 가질 때는 부정확할 수 있다.
2. 진공 상태 가정: 매질이 있는 경우 유전율을 고려해야 한다.
3. 상대론적 효과 무시: 매우 빠르게 움직이는 전하에 대해서는 부정확하다.

## 쿨롱 법칙과 중력의 유사성

쿨롱의 법칙은 뉴턴의 중력 법칙과 수학적 형태가 매우 유사하다:

$$ F_g = G \frac{m_1 m_2}{r^2} \quad \text{vs.} \quad F_e = k \frac{q_1 q_2}{r^2} $$

이 유사성은 전기력과 중력의 근본적인 연관성을 시사하며, 통일장 이론 연구의 동기가 되었다.

쿨롱의 법칙은 전자기학의 기본 원리로, 전하를 띤 입자들 사이의 상호작용을 이해하는 데 핵심적인 역할을 한다. 이는 물질의 구조부터 현대 기술의 다양한 응용에 이르기까지 광범위한 영향을 미친다.

[^1]: 진공상태에서의 비유전율은 1. 