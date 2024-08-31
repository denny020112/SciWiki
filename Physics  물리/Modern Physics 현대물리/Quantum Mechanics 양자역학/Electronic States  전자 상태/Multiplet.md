---
aliases:
  - Multiplet
  - Multiplicity
  - 다중항
category:
  - 물리학
  - 양자역학
related_concepts:
  - 고전역학
  - 물리
  - 스핀
  - 각운동량
tags:
  - 물리
  - 화학
  - 양자화학
  - 양자역학
  - 물리화학
  - 계산화학
  - 자기화학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 다중항 (Multiplet)

## 정의 및 개요
$$\text{Multiplicity (multiplet)} = 2S + 1$$

다중항은 다중도로인해 발생하는 분광학적 패턴, 혹은 다중도 자체를 뜻한다. 2S+1로 계산된다. 단순히 스펙트럼의 해석에서만 쓰이는 개념은 아닌데, 이는 다중항은 가능한 전자의 배치와 전자가 가질 수 있는 에너지 준위를 설명하기 때문이다.

다중항은 물질의 자기적 성질을 설명하는데 직접적으로 사용되기도 하며, 또한 다중도 상태에 따라 물질이 다른 반응성을 가지는 경우 또한 존재한다.

## 주요 다중항

1. 단일항 (Singlet)
   - S = 0
   - 다중항 = 2(0) + 1 = 1
   - 모든 전자의 스핀이 쌍을 이룸
   - 예: 헬륨 원자의 기저 상태 (1s²)

2. 이중항 (Doublet)
   - S = 1/2
   - 다중항 = 2(1/2) + 1 = 2
   - 홀전자가 1개 존재
   - 예: 수소 원자, 알칼리 금속 원자들의 기저 상태

3. 삼중항 (Triplet)[^1]
   - S = 1
   - 다중항 = 2(1) + 1 = 3
   - 평행한 스핀을 가진 두 개의 홀전자 존재
   - 예: 산소 분자의 기저 상태

4. 사중항 (Quartet)
   - S = 3/2
   - 다중항 = 2(3/2) + 1 = 4
   - 세 개의 평행한 스핀을 가진 홀전자 존재
   - 예: 질소 원자의 기저 상태

## 미세 구조 (Fine Structure)

미세 구조는 전자의 스핀과 궤도 각운동량의 상호작용으로 인해 발생하는 에너지 준위의 분리를 말한다. 이때 다중도에 의해 발생한 여러 선의 스펙트럼 혹은 분광 스펙트럼의 여러 피크를 다중항이라고 한다. 

1. 단일항 (Singlet):
    - 미세 구조가 나타나지 않음
    - 단일 스펙트럼 선으로 관찰
2. 이중항 이상 (Doublet, Triplet, etc.):
    - 미세 구조로 인한 스펙트럼 선의 분리 발생
    - 다중항 수에 따라 분리된 선의 개수가 결정됨

### 예시 1: 나트륨의 이중항

![[sodium doublet.png|400]]
나트륨 원자의 바닥상태 전자 배치: $[\text{Ne}]3s^{1}$

1. 총 스핀 S = 1/2 (홀전자 1개)
2. 다중항 = 2S + 1 = 2 (이중항)

나트륨 D-선의 스펙트럼:

- 3p → 3s 전이에서 관찰
- 두 개의 근접한 선으로 나타남: D₁ (589.6 nm)과 D₂ (589.0 nm)
- 이 분리는 3p 상태의 미세 구조 때문에 발생
    - ²P₁/₂ → ²S₁/₂ (D₁ 선)
    - ²P₃/₂ → ²S₁/₂ (D₂ 선)

### 예시 2: Orthohelium과 Parahelium

헬륨 원자의 들뜬 상태는 orthohelium과 parahelium으로 구분된다.

1. Parahelium (단일항 상태):
    - 두 전자의 스핀이 반대방향 (↑↓)
    - S = 0, 다중항 = 1
    - 예: 1s2s ¹S₀ 상태
2. Orthohelium (삼중항 상태):
    - 두 전자의 스핀이 같은 방향 (↑↑)
    - S = 1, 다중항 = 3
    - 예: 1s2s ³S₁ 상태

스펙트럼 특성:

- Parahelium: 단일 스펙트럼 선으로 관찰
- Orthohelium: 삼중항 상태의 미세 구조로 인해 여러 개의 근접한 선으로 분리되어 관찰

이 두 상태 간의 전이는 스핀 선택 규칙($\Delta S = 0$)에 의해 금지되어 있어, 서로 독립적인 스펙트럼 계열을 형성한다.


## 훈트의 규칙과의 관계

훈트의 첫 번째 규칙은 주어진 전자 배치에서 가장 큰 다중항을 가진 상태가 가장 낮은 에너지를 갖는다고 말한다. 이는 다중항의 개념이 원자와 분자의 기저 상태를 이해하는 데 얼마나 중요한지를 보여준다.





[^1]: 단일항-삼중항 전이는 많은 광화학 반응에서 중요한 지표로써 역할한다.