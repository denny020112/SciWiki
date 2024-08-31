---
alias: [Term Symbol, Spectroscopic Term]
subject: 양자화학, 분광학
related_topics: [전자 배치, 스핀-궤도 결합, 훈트 규칙]
tags: [물리화학, 원자 스펙트럼, 전자 상태]
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 항 표기법 (Term Symbol)

## 정의 및 개요

항 표기법은 원자나 분자의 전자 상태를 간결하게 표현하는 방식이다. 이는 전자의 각운동량, 스핀, 그리고 전체 각운동량 정보를 포함한다.

## 일반 형식

$$^{2S+1}L_J$$

여기서:
- $2S+1$: 스핀 다중도
- $L$: 궤도 각운동량 (S, P, D, F, ...)
- $J$: 전체 각운동량 양자수

## 구성 요소 설명

### 스핀 다중도 (2S+1)
- $S$는 총 스핀 각운동량
- 값: 1 (singlet), 2 (doublet), 3 (triplet) 등

### 궤도 각운동량 (L)
- 값에 따른 기호:
  - L = 0: S (Sharp)
  - L = 1: P (Principal)
  - L = 2: D (Diffuse)
  - L = 3: F (Fundamental)
  - L ≥ 4: 알파벳 순서로 G, H, I, ...

### 전체 각운동량 (J)
- $J = |L - S|, |L - S| + 1, ..., L + S$

## 예시

### 헬륨 원자 기저 상태
- 전자 배치: 1s²
- 항 표기: ¹S₀
  - S = 0 (모든 전자 쌍을 이룸)
  - L = 0 (s 궤도)
  - J = 0

### 탄소 원자 기저 상태
- 전자 배치: 1s² 2s² 2p²
- 항 표기: ³P₀
  - S = 1 (훈트 규칙에 따라 2개의 홀전자)
  - L = 1 (P 상태)
  - J = 0 (가능한 J 값 중 최소값)

### 나트륨 원자 들뜬 상태
- 전자 배치: 1s² 2s² 2p⁶ 3p¹
- 항 표기: ²P₃/₂
  - S = 1/2 (하나의 홀전자)
  - L = 1 (P 상태)
  - J = 3/2 (가능한 J 값 중 최대값)

## 중요성

1. 스펙트럼 해석: 전이 규칙 이해와 예측
2. 원자/분자 상태 분류: 에너지 준위 구분
3. 화학 결합 이해: 분자 형성 시 전자 상태 변화 추적

## 주의사항

1. 다전자 시스템에서는 전자 간 상호작용으로 복잡해질 수 있다.
2. 무거운 원자에서는 스핀-궤도 결합이 중요해져 LS 결합 근사가 부적절할 수 있다.
3. 분자에서는 추가적인 양자수가 필요할 수 있다.

## 결론

항 표기법은 원자와 분자의 전자 상태를 간결하고 정확하게 표현하는 강력한 도구다. 이를 통해 복잡한 전자 구조와 스펙트럼을 이해하고 예측할 수 있다. 양자화학과 분광학 연구에 필수적인 개념이다.