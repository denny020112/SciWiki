---
aliases:
  - Rigid Rotator
  - Rigid Rotor Model
  - 강체 회전자
category:
  - 양자역학
  - 분광학
  - 물리학
related_topics:
  - 각운동량
  - 구면 조화 함수
  - 양자수
tags:
  - 양자역학
  - 분광학
  - 물리
  - 화학
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

# 회전 상태 (Rotational State)

## 정의 및 개요

양자역학에서의 회전 상태는 주로 전자기파 혹은 전자기 복사가 분자 및 입자에 돌림힘(Torque)를 가했을 때를 일컫는다. 

주로 이러한 상태를 계산하기 위해서는 간단한 강체 회전자를 가정한다. 구형 강체 회전자가 아닌 경우에는 해석적인 해를 찾기 힘들다.

강체 회전자는 내부 진동이 없이 회전만 하는 이상적인 분자 모델이다. 두 개의 원자가 고정된 거리를 유지한 채 회전하는 이원자 분자가 대표적인 예다.

## 물리적 특성 및 상세
### 해밀토니안

강체 회전자의 해밀토니안은 다음과 같다:

$$H = \frac{L^2}{2I}$$

여기서:
- $L$은 각운동량 연산자
- $I$는 관성 모멘트 ($I = \mu r^2$, $\mu$는 환산 질량, $r$은 원자 간 거리)
	- 증명: $$\begin{flalign} \\ I&=\sum_{i=1}^Nm_ir_i^2\\ &= m_Ax^2+m_B(r_{AB}-x)^2\\ &=\frac{m_Am_B}{m_A+m_B}r^2_{AB}\\  &\text{let, reduced mass}=\mu=\frac{m_Am_B}{m_A+m_B}  \\&   \Rightarrow \therefore I=\mu r^2  &&  \end{flalign} $$

구면 좌표계에서 각운동량 연산자 $L^2$는 다음과 같이 표현된다:

$$L^2 = -\hbar^2 \left[\frac{1}{\sin\theta}\frac{\partial}{\partial\theta}\left(\sin\theta\frac{\partial}{\partial\theta}\right) + \frac{1}{\sin^2\theta}\frac{\partial^2}{\partial\phi^2}\right]$$

### 슈뢰딩거 방정식

$$-\frac{\hbar^2}{2I}\left[\frac{1}{\sin\theta}\frac{\partial}{\partial\theta}\left(\sin\theta\frac{\partial\psi}{\partial\theta}\right) + \frac{1}{\sin^2\theta}\frac{\partial^2\psi}{\partial\phi^2}\right] = E\psi$$

회전 상태의 슈뢰딩거 방정식. 강체 회전자를 가정하고 푼다.
일반적인 해밀토니언에서 구면 좌표계로 변환함으로써 구한 회전 해밀토니언을 슈뢰딩거 방정식에 대신 적용함으로써 찾을 수 있다.. 
여기서 $\psi(\theta,\phi)$는 파동함수다. 구형이 아닌 강체 회전자의 경우에는 해를 구할 수 없다
#### 증명

##### 1. 일반 슈뢰딩거 방정식

시간 독립 슈뢰딩거 방정식의 일반적인 형태:

$$\hat{H}\Psi = E\Psi$$

여기서 $\hat{H}$는 해밀토니안 연산자, $\Psi$는 파동함수, $E$는 에너지 고유값이다.

##### 2. 회전 운동의 해밀토니안

강체 회전자 가정 시 회전 운동의 해밀토니안:

$$\hat{H} = \frac{\hat{L}^2}{2I}$$

여기서 $\hat{L}$은 각운동량 연산자, $I$는 관성 모멘트이다.

##### 3. 구면 좌표계로의 변환

각운동량 연산자 $\hat{L}^2$를 구면 좌표계 $(r, \theta, \phi)$로 표현:

$$\hat{L}^2 = -\hbar^2 \left[\frac{1}{\sin\theta}\frac{\partial}{\partial\theta}\left(\sin\theta\frac{\partial}{\partial\theta}\right) + \frac{1}{\sin^2\theta}\frac{\partial^2}{\partial\phi^2}\right]$$

##### 4. 회전 상태의 슈뢰딩거 방정식

구면 좌표계로 표현한 회전 상태의 슈뢰딩거 방정식:

$$-\frac{\hbar^2}{2I} \left[\frac{1}{\sin\theta}\frac{\partial}{\partial\theta}\left(\sin\theta\frac{\partial\Psi}{\partial\theta}\right) + \frac{1}{\sin^2\theta}\frac{\partial^2\Psi}{\partial\phi^2}\right] = E\Psi$$

##### 5. 변수 분리

파동함수를 $\Psi(\theta,\phi) = \Theta(\theta)\Phi(\phi)$로 분리:

$$\frac{1}{\Theta}\frac{1}{\sin\theta}\frac{d}{d\theta}\left(\sin\theta\frac{d\Theta}{d\theta}\right) + \frac{1}{\Phi}\frac{1}{\sin^2\theta}\frac{d^2\Phi}{d\phi^2} = -\frac{2IE}{\hbar^2}$$

##### 6. ϕ에 대한 방정식

$$\frac{d^2\Phi}{d\phi^2} = -m^2\Phi$$

해: $$\Phi(\phi) = e^{\pm im\phi}$$

여기서 $m$은 정수이다.

##### 7. θ에 대한 방정식

$$\frac{1}{\sin\theta}\frac{d}{d\theta}\left(\sin\theta\frac{d\Theta}{d\theta}\right) + \left[\frac{2IE}{\hbar^2} - \frac{m^2}{\sin^2\theta}\right]\Theta = 0$$

이는 르장드르 방정식의 형태이며, 해는 르장드르 다항식으로 주어진다.

##### 8. 최종 해

회전 상태의 슈뢰딩거 방정식의 최종 해:

$$\Psi_{l,m}(\theta,\phi) = N_{l,m}P_l^m(\cos\theta)e^{im\phi}$$

여기서 $N_{l,m}$은 규격화 상수, $P_l^m$은 르장드르 다항식이다. 

에너지 고유값:

$$E_l = \frac{\hbar^2}{2I}l(l+1)$$

여기서 $l$은 각운동량 양자수이다.

### 에너지

슈뢰딩거 방정식의 해를 구하면 회전 상태의 에너지 준위를 얻을 수 있다:

$$E_J = \frac{\hbar^2}{2I}J(J+1)$$

여기서 $J$는 [[Term Symbol#전체 각운동량 (J)|전체 각운동량 양자수]]로, $J = 0, 1, 2, ...$의 값을 가진다.

### 구면 조화 함수

강체 회전자의 파동함수는 구면 조화 함수(Spherical Harmonics)로 표현된다:

$$Y_l^m(\theta,\phi) = (-1)^m\sqrt{\frac{(2l+1)}{4\pi}\frac{(l-m)!}{(l+m)!}}P_l^m(\cos\theta)e^{im\phi}$$

여기서:
- $l$은 각운동량 양자수 ($l = J$)
- $m$은 각운동량의 z-성분 양자수 ($m = -l, -l+1, ..., l-1, l$)
- $P_l^m$은 연관 르장드르 다항식

### 강체 회전자에서의 축퇴

#### 방향 축퇴 (Directional Degeneracy)

각 $J$ 값에 대해 $2J+1$개의 $m$ 값이 존재한다. 이는 각운동량 벡터가 공간상에서 취할 수 있는 방향의 수를 나타낸다.

#### 에너지 축퇴

에너지는 $J$에만 의존하고 $m$에는 의존하지 않는다. 따라서 같은 $J$ 값을 가진 모든 상태는 동일한 에너지를 가진다. 이를 에너지 축퇴라고 한다.

#### 축퇴도 (Degeneracy)

주어진 $J$에 대한 축퇴도는 $2J+1$이다. 예를 들어:
- $J=0$: 축퇴도 1
- $J=1$: 축퇴도 3
- $J=2$: 축퇴도 5

#### 축퇴의 물리적 의미

- 공간 등방성: 회전의 방향이 에너지에 영향을 주지 않음
- 각운동량 보존: 회전 축의 방향이 보존됨

