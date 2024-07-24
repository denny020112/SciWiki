---
alias: [Operator, 작용소, 연산자]
category: [선형대수학, 함수해석학, 양자역학]
related_concepts: [선형 변환, 함수, 행렬, 고유값, 고유벡터]
tags: [수학, 물리학, 선형대수학, 양자역학]
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 연산자

## 정의

연산자는 한 수학적 객체를 다른 수학적 객체로 변환하는 함수 또는 규칙이다. 특히 선형 연산자는 벡터 공간에서 정의되며, 다음 성질을 만족한다:

$$ T(a\mathbf{x} + b\mathbf{y}) = aT(\mathbf{x}) + bT(\mathbf{y}) $$

여기서 $T$는 연산자, $a,b$는 스칼라, $\mathbf{x},\mathbf{y}$는 벡터이다.

## 중요 성질

1. 선형성: 선형 연산자는 덧셈과 스칼라 곱에 대해 분배법칙을 만족한다.
2. 가역성: 역연산자가 존재하는 경우 연산자는 가역적이다.
3. 에르미트성[^1]: $\langle T\mathbf{x}, \mathbf{y} \rangle = \langle \mathbf{x}, T\mathbf{y} \rangle$를 만족하는 경우 에르미트 연산자라 한다.
4. 유니터리성: $T^*T = TT^* = I$를 만족하는 경우 유니터리 연산자라 한다.
5. 콤팩트성: 유계 집합을 콤팩트 집합으로 보내는 연산자를 콤팩트 연산자라 한다.

## 주요 정리

1. 스펙트럼 정리
   증명: 에르미트 연산자 $T$는 $T = \sum_i \lambda_i |\phi_i\rangle\langle\phi_i|$로 표현할 수 있다.

2. 폰 노이만의 스펙트럼 정리
   증명: 유계 정규 연산자 $T$는 $T = \int_{\sigma(T)} \lambda dE(\lambda)$로 표현할 수 있다.

3. 리스-프리드리히 정리
   증명: 콤팩트 자기수반 연산자의 고유값은 0으로 수렴하는 수열을 이룬다.

## 응용

- 양자역학에서의 물리량 표현
- 미분 방정식의 해법
- 신호 처리 및 이미지 분석
- 데이터 압축
- 기계 학습의 선형 변환

## 관련 개념

- 행렬
- 벡터 공간
- 고유값과 고유벡터
- 함수 공간
- 스펙트럼 이론

## 예제

1. 미분 연산자
   해설: $D = \frac{d}{dx}$는 선형 연산자이다. $D(af(x) + bg(x)) = af'(x) + bg'(x)$

2. 투영 연산자
   해설: $P = \mathbf{v}\mathbf{v}^T/\|\mathbf{v}\|^2$는 벡터 $\mathbf{v}$에 대한 투영 연산자이다.

## 역사적 배경

연산자 이론은 19세기 말과 20세기 초에 발전했다. 힐베르트, 폰 노이만, 리스 등이 주요 기여를 했으며, 양자역학의 발전과 함께 그 중요성이 더욱 부각되었다.

## 시각화

[선형 변환의 기하학적 표현]
[스펙트럼의 시각화]
[연산자의 행렬 표현]

## 계산 방법

1. 행렬 표현: 유한 차원에서 연산자를 행렬로 표현
2. 고유값 분해: $T = \sum_i \lambda_i \mathbf{v}_i\mathbf{v}_i^T$
3. 특이값 분해: $T = U\Sigma V^*$
4. 함수 공간에서의 적분 표현: $Tf = \int K(x,y)f(y)dy$

## 주의사항

- 무한 차원 공간에서는 유한 차원과 다른 성질이 나타날 수 있다.
- 비유계 연산자의 경우 정의역과 치역에 주의해야 한다.
- 비선형 연산자의 경우 선형 연산자와는 다른 접근이 필요하다.

## 참고 문헌

1. Reed, M., & Simon, B. (1980). Methods of Modern Mathematical Physics: Functional Analysis. Academic Press.
2. Kreyszig, E. (1978). Introductory Functional Analysis with Applications. John Wiley & Sons.
3. Rudin, W. (1991). Functional Analysis. McGraw-Hill.

## 추가 학습 자료

- MIT OpenCourseWare: Linear Algebra
- Coursera: Functional Analysis
- YouTube: 3Blue1Brown의 선형대수학 시리즈


[^1]: Hermitian;  허미티안.