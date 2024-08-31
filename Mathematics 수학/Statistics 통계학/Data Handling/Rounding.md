---
aliases:
  - 반올림
  - 반내림
  - 올림
category:
  - 수학
  - 통계
related_concepts:
  - 유효숫자
  - 과학적 표기법
  - 오차
tags:
  - 수치해석
  - 수학
  - 통계적
  - 데이터
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 반올림 (Rounding)

## 정의

반올림은 수를 가장 가까운 정수나 원하는 소수점 자리로 근사하는 과정이다. 이는 계산을 간소화하거나 측정의 정밀도를 표현하는 데 사용된다.

## 기본 규칙

1. 5 미만은 내림
2. 5 초과는 올림
3. 정확히 5일 경우, 상황에 따라 다른 규칙 적용

## 반올림 방법들

### 일반적인 반올림 (Round-off)

가장 흔한 방법으로, 5 이상은 올림, 5 미만은 내림한다.

예시:
- 3.14159 → 3.14 (소수점 둘째 자리로 반올림)
- 2.5 → 3
- 2.4 → 2

### 은행가 반올림 (Banker's Rounding)

5일 경우 가장 가까운 짝수로 반올림한다. 이는 편향을 줄이는 데 효과적이다.

예시:
- 2.5 → 2
- 3.5 → 4
- 2.45 → 2.4
- 2.55 → 2.6

### 올림 (Round-up)

항상 다음 큰 수로 올린다.

예시:
- 3.14159 → 3.15 (소수점 둘째 자리로 올림)
- 2.1 → 3 (정수로 올림)

### 내림 (Round-down)

항상 다음 작은 수로 내린다.

예시:
- 3.14159 → 3.14 (소수점 둘째 자리로 내림)
- 2.9 → 2 (정수로 내림)



## 주의사항

1. 연속적인 반올림 시 오차 누적 가능
2. 큰 데이터셋에서는 반올림 방식에 따라 결과가 크게 달라질 수 있음
3. 특정 분야(예: 재무)에서는 법규나 관행에 따른 특정 반올림 방식 사용

## 관련 개념

- [[Significant Figures]]
- [[Scientific Notation]]
- [[Truncation]]

## 참고문헌

1. Goldberg, D. (1991). What every computer scientist should know about floating-point arithmetic. ACM Computing Surveys, 23(1), 5-48.
2. Higham, N. J. (2002). Accuracy and stability of numerical algorithms. SIAM.