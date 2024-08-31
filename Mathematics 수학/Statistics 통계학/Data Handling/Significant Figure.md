---
aliases:
  - 유효숫자
  - 유효자릿수
category:
  - 수학
related_concepts:
  - 과학적 표기법
  - 반올림
  - 측정 불확도
tags:
  - 데이터
  - 수치해석
  - 수학
  - 통계학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 유효숫자 (Significant Figures)

## 정의

유효숫자는 측정값이나 계산 결과에서 의미 있는 자릿수를 나타낸다. 이는 측정의 정밀도를 적절하고 명확히[^1] 표현하는데 도움이 되며, 계산 결과의 신뢰성을 나타내는 데 사용된다. 

## 규칙

1. 0이 아닌 모든 숫자는 유효하다.
2. 숫자 사이의 0은 유효하다.
3. 맨 앞의 0은 유효하지 않다.
4. 소수점 뒤의 0은 유효하다.
5. 정수의 맨 뒤 0은 애매할 수 있으므로 과학적 표기법을 사용하여 명확히 한다.

### 주의사항

1. 정확한 수(예: 2π)는 유효숫자 계산에 포함되지 않는다.
2. 중간 계산 결과는 최종 결과보다 1자리 더 많은 유효숫자를 유지한다.[^2]
3. 로그를 취할 때는 유효숫자의 수가 아닌 소수점 이하 자릿수를 고려한다.

## 예시

1. 1234 : 4개의 유효숫자
2. 1.234 : 4개의 유효숫자
3. 0.00123 : 3개의 유효숫자
4. 1.230 : 4개의 유효숫자
5. 1200 : 2개 또는 4개의 유효숫자 (애매함)
   $1.2 \times 10^3$ (2개의 유효숫자)
   $1.200 \times 10^3$ (4개의 유효숫자)

## 계산 방법

1. 덧셈과 뺄셈: 결과는 가장 적은 소수점 자리수를 가진 피연산자와 같은 소수점 자리수를 갖는다.
   
   $23.45 + 1.004 = 24.454 ≈ 24.45$

2. 곱셈과 나눗셈: 결과는 가장 적은 유효숫자를 가진 피연산자와 같은 개수의 유효숫자를 갖는다.
   
   $2.34 × 1.2 = 2.808 ≈ 2.8$


## 관련 개념

- [[Scientific Notation|과학적 표기법]]
- [[Rounding|반올림]]
- [[Measurement Uncertainty]]

## 참고문헌

1. Taylor, J. R. (1997). An Introduction to Error Analysis. University Science Books.
2. Bevington, P. R., & Robinson, D. K. (2003). Data Reduction and Error Analysis for the Physical Sciences. McGraw-Hill.



[^1]: 과도한 정밀도 또한 지양된다.
[^2]: 뒤에 추가로 유지하는 숫자는 Guard digit이라고 한다.
