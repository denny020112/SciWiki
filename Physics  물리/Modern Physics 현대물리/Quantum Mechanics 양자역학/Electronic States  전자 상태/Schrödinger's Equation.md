---
aliases:
  - Schrödinger equation
  - 파동방정식
category:
  - 양자역학
  - 물리화학
related_concepts:
  - 파동함수
  - 연산자
  - 고유값
  - 고유함수
  - 양자화
tags:
  - 양자역학
  - 물리
  - 양자화학
  - 수학
  - 미적분학
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

# 슈뢰딩거 방정식 (Schrödinger Equation)

## 정의

슈뢰딩거 방정식은 양자역학적 시스템의 파동함수를 결정하는 방정식이다. 이 방정식은 시스템의 전체 에너지를 운동 에너지와 퍼텐셜 에너지의 합, 즉 [[Hamiltonian|해밀토니언]]을 이용하여 표현하며, 파동함수를 통해 시스템의 상태를 기술한다.

### 시간 독립형 슈뢰딩거 방정식

시간에 따라 변하지 않는 정상상태(stationary state)를 기술하는 방정식이다.

$$ \hat{H}\Psi = E\Psi $$

여기서:
- $\hat{H}$: 해밀토니안 연산자
- $\Psi$: 파동함수
- $E$: 시스템의 전체 에너지

1차원에서의 구체적인 형태:

$$ -\frac{\hbar^2}{2m}\frac{d^2\Psi}{dx^2} + V(x)\Psi = E\Psi $$

여기서:
- $\hbar$: 축약된 플랑크 상수
- $m$: 입자의 질량
- $V(x)$: 퍼텐셜 에너지 함수

### 시간 발전형 슈뢰딩거 방정식

시간에 따른 시스템의 변화를 기술하는 방정식이다.

$$ i\hbar\frac{\partial\Psi}{\partial t} = \hat{H}\Psi $$

여기서:
- $i$: 허수단위
- $t$: 시간

1차원에서의 구체적인 형태:

$$ i\hbar\frac{\partial\Psi}{\partial t} = -\frac{\hbar^2}{2m}\frac{\partial^2\Psi}{\partial x^2} + V(x)\Psi $$



## 퍼텐셜 우물 (Potential Well) 

퍼텐셜 우물은 입자가 갇혀있는 특정 영역을 나타내는 퍼텐셜 에너지 모델이다. 이는 양자역학의 기본 개념을 이해하는 데 중요한 역할을 한다. 
### 1차원 무한 퍼텐셜 우물 

![[1d potential well.png|350]]


길이가 a인 1차원 공간에 입자가 있고, 
퍼텐셜은 다음과 같은 경계조건을 바탕으로 우물과 같이 입자를 가둔다.

$$V(x) = \begin{cases} 
0 & \text{for } 0 < x < a \\
\infty & \text{elsewhere}
\end{cases}$$


이때 시간 독립 슈뢰딩거 방정식은 다음과 같다.

$$-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} + V(x)\psi = E\psi$$


퍼텐셜 우물 내부$(0<x<a)$를 먼저 고려해보자.
우물 내부에서 $V(x) = 0$이므로:
$$-\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2} = E\psi$$

이를 정리하면:
$$\frac{d^2\psi}{dx^2} + \frac{2mE}{\hbar^2}\psi = 0$$

여기서 $k^2 = \frac{2mE}{\hbar^2}$로 치환하면 다음과 같은 식의 형태로 정리가 된다.

$$\frac{d^2\psi}{dx^2} + k^2\psi = 0$$

우물 내부의 상황을 고려했을 때의 조건에 맞는 일반해는 다음과 같을 것이다.

$$\psi(x) = A\sin(kx) + B\cos(kx)$$


구한 일반해에 처음에 주어진 경계조건을 각각 적용한다.

1) $\psi(0) = 0$ 조건 적용:
   
   $\psi(0) = A\sin(0) + B\cos(0) = B = 0$

   따라서 $B = 0$이고, $\psi(x) = A\sin(kx)$

2) $\psi(a) = 0$ 조건 적용:
   
   $\psi(a) = A\sin(ka) = 0$

   $\sin(ka) = 0$이어야 하므로, $ka = n\pi$ (n은 정수)



$ka = n\pi$에서 $k = \frac{n\pi}{a}$

$k^2 = \frac{2mE}{\hbar^2}$이므로:

$$\frac{2mE}{\hbar^2} = (\frac{n\pi}{a})^2$$

이를 E에 대해 정리하면:

$$E_n = \frac{n^2\pi^2\hbar^2}{2ma^2}$$

여기서 n은 1, 2, 3, ... 의 값을 가질 수 있는 양의 정수이다.

구한 조건들을 정리하여 적용하면 파동함수는 다음 형태를 가진다:

$$\psi_n(x) = A\sin(\frac{n\pi x}{a})$$

정규화 조건을 적용하면:

$$\int_0^a |\psi_n(x)|^2 dx = 1$$

$$A^2\int_0^a \sin^2(\frac{n\pi x}{a}) dx = 1$$

적분을 계산하면:

$$A^2 \cdot \frac{a}{2} = 1$$

따라서 $A = \sqrt{\frac{2}{a}}$

**완전한 해는:**
$$\psi_n(x) = \sqrt{\frac{2}{a}}\sin(\frac{n\pi x}{a})$$

에너지 준위 $E_n$은 n의 제곱에 비례하며, 파동함수 $\psi_n(x)$는 정현파[^1] 형태를 가진다.

### 유한 퍼텐셜 우물 

현실적인 시스템을 더 잘 모델링하는 퍼텐셜 우물로, 입자가 우물 밖으로 터널링할 확률이 존재한다. 퍼텐셜 에너지: $$ V(x) = \begin{cases} 0 & \text{if } 0 < x < a \\ V_0 & \text{otherwise} \end{cases} $$ 이 경우, 해석적 해를 구하기 어려우며 주로 수치적 방법을 사용한다. 

### 3차원 퍼텐셜 상자 (Infinite Potential Cubic Box)

모든 변의 길이가 $L$[^2]인 정육면체 상자를 가정해보자.
![[particle in 3d box.png|500]]
상자 내부에서는 $V = 0$, 상자 외부에서는 $V = \infty$로 경계 조건을 설정한다

이때의 해밀토니언은 다음과 같다.
$$-\frac{\hbar^2}{2m}\left(\frac{\partial^2\psi}{\partial x^2} + \frac{\partial^2\psi}{\partial y^2} + \frac{\partial^2\psi}{\partial z^2}\right) = E\psi$$

변수를 분리하고,
$$\psi(x,y,z) = X(x)Y(y)Z(z)$$
각 방향에 대해 동일한 해를 먼저 구한 뒤[^3] [^4],
$$X(x) = A\sin(k_xx), \quad k_x = \frac{n_x\pi}{L}$$
$$Y(y) = B\sin(k_yy), \quad k_y = \frac{n_y\pi}{L}$$
$$Z(z) = C\sin(k_zz), \quad k_z = \frac{n_z\pi}{L}$$

3차원 파동함수로 합쳐준다.

$$\psi_{n_x,n_y,n_z}(x,y,z) = A\sin(\frac{n_x\pi x}{L})\sin(\frac{n_y\pi y}{L})\sin(\frac{n_z\pi z}{L})$$

1차원 퍼텐셜 우물에서의 경우와 유사하게 **에너지 준위** 기준으로 정리해주면:

$$E_{n_x,n_y,n_z} = \frac{\hbar^2\pi^2}{2mL^2}(n_x^2 + n_y^2 + n_z^2)$$

파동함수의 특성을 이용해 **정규화**를 해주면:

$$\psi_{n_x,n_y,n_z}(x,y,z) = \sqrt{\frac{8}{L^3}}\sin(\frac{n_x\pi x}{L})\sin(\frac{n_y\pi y}{L})\sin(\frac{n_z\pi z}{L})$$

#### 기저 에너지 준위

기저 상태 혹은 바닥상태는 $(n_x,n_y,n_z) = (1,1,1)$, 즉 모든 축에 대해 준위가 제일 낮은 상태일 것이고, 그대로 구해놓은 에너지 준위 식에 넣으면 다음과 같이 나타날 것이다.
   $$E_{1,1,1} = \frac{3\hbar^2\pi^2}{2mL^2}$$
#### 축퇴 (Degeneracy)

예를 들어, $(2,1,1)$, $(1,2,1)$, $(1,1,2)$는 모두 같은 에너지를 가진다. 이렇게 같은 에너지 준위룰 가지는 다른 상태들을 축퇴 에너지 상태라고 한다.
$$E_{2,1,1} = E_{1,2,1} = E_{1,1,2} = \frac{6\hbar^2\pi^2}{2mL^2}$$

## 주요 응용

1. 수소 원자의 에너지 준위 계산
2. 입자의 터널링 현상 설명
3. 조화 진동자 모델
4. 분자의 전자 구조 계산
3. 측정 문제 (파동함수 붕괴)

## 여담

- 슈뢰딩거 방정식은 양자역학의 기본 방정식이지만, 실제 다체 상황에서는 근사적 방법을 사용해야 한다. 밀도 범함수 이론(DFT), 보른-오펜하이며 근사, 평균장 이론 같은 방법들이 복잡한 시스템의 해를 구하는 데 널리 사용된다.
- 슈뢰딩거 방정식 자체로는 상대론적 효과를 고려한 계산을 할 수가 없다. 이를 위해 나온것이 디랙 방정식.



## 관련 개념
- [[파동함수]]
- [[operator|연산자]]
- [[고유값 문제]]
- [[불확정성 원리]]

## 참고문헌

1. Griffiths, D.J. (2018). Introduction to Quantum Mechanics. Cambridge University Press.
2. Shankar, R. (2011). Principles of Quantum Mechanics. Springer Science & Business Media.




[^1]: 사인파
[^2]: a 라고 표기하기도 한다.
[^3]: 여기서 n<sub>x</sub>, n<sub>y</sub>, n<sub>z</sub>는 양의 정수이다.
[^4]: 정육면체를 가정했기 때문에 가능한 단순화이다.
