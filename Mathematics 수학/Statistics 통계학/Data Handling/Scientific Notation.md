---
alias: [과학적 표기법, 지수 표기법]
category: [수학, 과학]
related_concepts: [유효숫자, 반올림, 지수]
tags: [표기법, 수치해석]
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 과학적 표기법 (Scientific Notation)

## 정의

과학적 표기법은 매우 크거나 매우 작은 수를 간단하게 표현하는 방법이다. 이 표기법에서는 수를 1 이상 10 미만의 수와 10의 거듭제곱의 곱으로 나타낸다.

## 기본 형식

$$a \times 10^n$$

여기서 $1 \leq |a| < 10$이고, $n$은 정수이다.

## 변환 방법

1. 소수점을 옮겨 $1 \leq |a| < 10$ 형태로 만든다.
2. 소수점을 옮긴 자릿수를 $n$으로 한다. 왼쪽으로 옮기면 양수, 오른쪽으로 옮기면 음수가 된다.

## 예시

1. 299,792,458 (빛의 속도, m/s) 
   = $2.99792458 \times 10^8$ m/s

2. 0.000000000000000000000001602 (전자의 전하량, C)
   = $1.602 \times 10^{-19}$ C

3. -0.00345 
   = $-3.45 \times 10^{-3}$

## 장점

1. 매우 크거나 작은 수를 간단히 표현할 수 있다.
2. 수의 크기를 쉽게 비교할 수 있다.
3. 계산이 용이하다.

## 계산 방법

1. 곱셈: 앞의 수를 곱하고 지수를 더한다.
   $(5 \times 10^3) \times (2 \times 10^4) = 10 \times 10^7 = 1 \times 10^8$

2. 나눗셈: 앞의 수를 나누고 지수를 뺀다.
   $(6 \times 10^5) \div (2 \times 10^2) = 3 \times 10^3$

## 주의사항

1. 음수의 경우, 앞의 수에 음수 부호를 붙인다.
2. 0은 $0 \times 10^0$로 표현한다.

## 관련 개념

- [[Significant Figures]]
- [[Rounding]]
- [[Exponents]]

## 참고문헌

1. Halliday, D., Resnick, R., & Walker, J. (2013). Fundamentals of Physics. John Wiley & Sons.
2. Young, H. D., Freedman, R. A., & Ford, A. L. (2015). University Physics with Modern Physics. Pearson.