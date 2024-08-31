---
aliases:
  - 보어의 원자 모델
  - Bohr model
  - 보어모델
  - 보어 모형
  - 행성 모형
category:
  - 양자화학
related_concepts:
  - 원자 구조
  - 전자 배치
  - 에너지 준위
tags:
  - 원자구조
  - 화학
  - 물리
  - 물리화학
  - 양자화학
  - 양자역학
---
```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 보어 모델

## 정의

1913년 닐스 보어가 제안한 원자 구조 모델. 이 모델은 원자핵 주위를 전자가 특정한 원형 궤도로 돌고 있다고 가정한다. 모형이 태양계와 비슷해 행성 모델이라고도 불린다.

## 기본 원리

1. 전자는 원자핵 주위의 양자화된, 불연속적이고 특정한 에너지 준위(궤도)[^1]에만 존재할 수 있다.
2. 전자가 한 에너지 준위에서 다른 준위로 이동할 때 에너지를 흡수하거나 방출한다.
3. 전자의 각운동량은 양자화되어 있다 ($L = n\hbar$; 여기서 n은 정수이다.)

### 에너지 준위

SI 단위계: $$E_n = -\frac{Z^2}{n^2} \cdot \frac{m_e e^4}{8\varepsilon_0^2h^2} = -\frac{Z^2}{n^2} \cdot 13.6 \text{ eV}$$

원자 단위계 (atomic units): $$E_n = -\frac{Z^2}{2n^2} \text{[Ha]}$$

여기서 1 $[Ha]$는[^3] 약 27.2 eV이다.

원자 단위계에서는 $m_e = e = \hbar = 4\pi\varepsilon_0 = 1$로 설정되어 식이 간단해진다.

### 궤도 반지름

SI 단위계: $$r_n = \frac{n^2}{Z} \cdot \frac{\varepsilon_0h^2}{\pi m_e e^2} = \frac{n^2}{Z} \cdot a_0$$

원자 단위계: $$r_n = \frac{n^2}{Z} \text{ Bohr}$$

여기서 1 Bohr는 $a_0$와 같으며, 약 0.529 Å이다.

### 전자 속도

SI 단위계: $$v_n = \frac{Z}{n} \cdot \frac{e^2}{2\varepsilon_0h}$$

원자 단위계: $$v_n = \frac{Z}{n}$$

## 보어 반지름 상수

보어 반지름 상수 $a_0$는 수소 원자의 바닥 상태 전자 궤도 반지름이다:

SI 단위계: $$a_0 = \frac{\varepsilon_0h^2}{\pi m_e e^2} \approx 0.529 \text{ Å}$$

원자 단위계: $a_0 = 1 \text{ Bohr}$

### $a_0$와 일반 $a$의 차이

- $a_0$: 수소 원자의 기저 상태 전자 궤도 반지름 (고정 상수)
- $a$: 임의의 원자와 에너지 준위에서의 전자 궤도 반지름

관계식: $$a = \frac{n^2}{Z} \cdot a_0$$
### $a_0$와 일반 $a$의 차이

- $a_0$: 수소 원자의 기저 상태 전자 궤도 반지름 (고정 상수)
- $a$: 임의의 원자와 에너지 준위에서의 전자 궤도 반지름

관계식: $$a = \frac{n^2}{Z} \cdot a_0$$

## 성공과 한계

### 성공

- 수소 원자의 선 스펙트럼 설명
- 리드버그 공식[^2] 이론적 설명 제공 $$\frac{1}{\lambda} = R(\frac{1}{n_f^2} - \frac{1}{n_i^2})$$

### 한계

- 다전자 원자의 스펙트럼 설명 불가
- 전자의 이중성(입자와 파동의 성질) 고려 부족


## 참고문헌

1. Bohr, N. (1913). On the Constitution of Atoms and Molecules. Philosophical Magazine, 26(151), 1-25.
2. Atkins, P., & de Paula, J. (2014). Atkins' Physical Chemistry (10th ed.). Oxford University Press.

[^1]: 껍질이라고도 한다.
[^2]: 뤼드베리 공식이라고도 한다
[^3]: Hartree. 하트리. 원자단위계에서의 에너지 단위.