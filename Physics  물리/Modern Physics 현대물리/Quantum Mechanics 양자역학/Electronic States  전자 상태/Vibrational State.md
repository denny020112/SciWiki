---
aliases:
  - 분자진동
  - 진동모드
category:
  - 양자화학
  - 분광학
related_concepts:
  - 회전상태
  - 전자상태
  - 슈뢰딩거 방정식
tags:
  - 분자구조
  - 에너지준위
  - 조화진동자
  - 양자역학
  - 양자화학
  - 물리
  - 화학
  - 물리화학
  - 분광학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 진동 상태 (Vibrational States)

## 정의

진동 상태는 분자 내 원자들의 주기적인 운동을 나타내는 양자역학적 상태이다. 이는 분자의 에너지와 구조에 중요한 영향을 미치며, 분광학적 특성을 결정하는 주요 요인 중 하나이다.

## 고전역학적 해석

### 조화 진동자 모델

고전역학에서 분자의 진동은 스프링으로 연결된 질점들의 운동으로 모델링할 수 있다. 이를 조화 진동자라고 한다.

운동 방정식: $m\frac{d^2x}{dt^2} = -kx$

여기서 $m$은 질량, $k$는 스프링 상수, $x$는 평형 위치로부터의 변위이다.

진동 주파수: $\nu = \frac{1}{2\pi}\sqrt{\frac{k}{m}}$

에너지: $E = \frac{1}{2}kA^2 = \frac{1}{2}m\omega^2A^2$

여기서 $A$는 진폭, $\omega = 2\pi\nu$는 각진동수이다.

## 양자역학적 해석

### 슈뢰딩거 방정식

1차원 조화 진동자의 슈뢰딩거 방정식:

$$-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} + \frac{1}{2}kx^2\psi = E\psi$$

### 에너지 준위

양자역학적 해석에서 진동 에너지는 양자화되어 있다:

$$E_v = \hbar\nu(v + \frac{1}{2}), \quad v = 0, 1, 2, ...$$

여기서 $v$는 진동 양자수, $\nu$ 는 고조파 주파수 (harmonic frequency)를 나타낸다.

$\nu$는 다음과 같다. $$\nu=\frac{1}{2\pi} \sqrt {\frac{k}{\mu}}$$
- $k$는 상수이다. 결합이 강한 경우 높은 값을 가진다
- $\mu$는 [[reduced mass|환산질량]]이다.  


### 파동함수

조화 진동자의 [[wave function|파동함수]]는 에르미트(Hermite) 다항식을 포함한다:

$$\psi_v(x) = N_v H_v(\alpha x)e^{-\alpha^2x^2/2}$$

여기서 $N_v$는 규격화 상수, $H_v$는 $v$차 에르미트 다항식, $\alpha = \sqrt{m\omega/\hbar}$이다.

## 진동상태의 특성

### 축퇴도/다중도

- 선형 분자: $3N-5$ 진동 모드 (N은 원자 수)
- 비선형 분자: $3N-6$ 진동 모드

### 영점 에너지 (Zero Point Energy)

양자역학적 조화 진동자의 최저 에너지 상태 ($v=0$)에서도 에너지가 존재한다:

$$E_0 = \frac{1}{2}\hbar\nu$$

### 선택규칙

적외선 분광학에서의 진동 전이 선택규칙: $\Delta v = \pm1$

## 다른 상태와의 관계

### 회전-진동 상호작용

실제 분자에서는 진동과 회전이 결합되어 있어, 에너지 준위가 약간 변형된다:

$$E_{v,J} = \hbar\nu(v + \frac{1}{2}) + BJ(J+1) - \alpha_e(v + \frac{1}{2})J(J+1)$$

여기서 $J$는 회전 양자수, $B$는 회전 상수, $\alpha_e$는 진동-회전 상호작용 상수이다.

### 전자-진동 상호작용

보른-오펜하이머(Born-Oppenheimer) 근사를 벗어나면 전자 상태와 진동 상태 사이의 상호작용을 고려해야 한다. 이는 얀-텔러(Jahn-Teller) 효과나 레너-텔러(Renner-Teller) 효과 등으로 나타날 수 있다.

## 비조화성

실제 분자에서는 비조화성이 존재하여, 에너지 준위가 조화 진동자 모델에서 벗어난다:

$$E_v = \hbar\omega(v + \frac{1}{2}) - \hbar\omega x_e(v + \frac{1}{2})^2 + ...$$

여기서 $x_e$는 비조화성 상수이다.

## 응용

- 적외선 분광학
- 라만 분광학
- 진동 원자가 이론 (VB theory)
- 분자 동력학 시뮬레이션

## 관련 개념

- [[Rotational States]]
- [[Electronic States]]
- [[Schrodinger Equation]]
- [[Spectroscopy]]

## 참고문헌

1. McQuarrie, D. A., & Simon, J. D. (1997). Physical Chemistry: A Molecular Approach. University Science Books.
2. Atkins, P. W., & Friedman, R. S. (2011). Molecular Quantum Mechanics. Oxford University Press.
3. Herzberg, G. (2013). Molecular Spectra and Molecular Structure: Vol. II - Infrared and Raman Spectra of Polyatomic Molecules. Van Nostrand.