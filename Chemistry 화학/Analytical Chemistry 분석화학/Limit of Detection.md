---
aliases:
  - limit of detection
  - LOD
  - 최소 검출량
  - 검출 한계
  - Detection Limit
category:
  - 분석화학
related_concepts:
  - 정량한계
  - 감도
  - 신호 대 잡음비
  - 검정곡선
tags:
  - 분석화학
  - 기기분석
  - 데이터
  - 화학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```

# 검출 한계 (Limit of Detection, LOD)

## 정의
분석 방법으로 검출 가능한 분석 대상 물질의 최소 농도 또는 양을 의미한다. 

## 핵심 원리
1. 바탕 신호와 통계적으로 구별 가능한 최소 신호 강도
2. 일반적으로 바탕 신호의 표준편차의 3배로 정의
3. 신호 대 잡음비(S/N)가 3인 지점

## 상세 설명
검출 한계는 분석 방법이나 기기의 성능을 나타내는 중요한 지표다. 이는 분석 대상 물질의 존재 여부를 확실히 판단할 수 있는 최소 농도를 의미한다. 검출 한계 이하의 농도에서는 신호가 바탕 잡음과 구별하기 어려워진다.

## 검출 한계의 계산
일반적으로 다음 식으로 계산한다:

$$ LOD = 3 \times \frac{s}{m} $$

여기서:
- s: 바탕 신호의 표준편차
- m: 검정곡선의 기울기 (감도)

## 검출 한계 결정 방법
1. 바탕 신호 방법
   - 여러 번의 바탕 측정 수행
   - 표준편차 계산
   - LOD = 평균 바탕 신호 + (3 × 표준편차)

2. 신호 대 잡음비 방법
   - S/N = 3인 지점의 농도 결정

3. 검정곡선 방법
   - 저농도 범위의 검정곡선 작성
   - y-절편의 표준편차 사용

## 예시
크로마토그래피에서 바탕 신호의 표준편차가 2 area units이고, 검정곡선의 기울기가 100 area units/ppm일 때:

$$ LOD = 3 \times \frac{2}{100} = 0.06 \text{ ppm} $$

## 검출 한계에 영향을 미치는 요인
1. 기기의 감도
2. 바탕 잡음의 크기
3. 시료 전처리 방법
4. 매트릭스 효과
5. 측정 조건 (온도, 압력 등)

## 검출 한계 개선 방법
1. 신호 증폭
2. 노이즈 감소
3. 시료 농축
4. 더 민감한 검출기 사용
5. 화학적 유도체화

## 관련 개념
- [[정량한계]]
- [[감도]]
- [[신호 대 잡음비]]
- [[검정곡선]]

## 응용 분야
1. 환경 분석: 오염물질 검출
2. 식품 안전: 잔류 농약, 중금속 분석
3. 임상 화학: 혈액, 소변 내 대사산물 분석
4. 법의학: 독성물질 분석

## 주의사항
1. 검출 한계는 물질의 존재 여부만 판단 가능
2. 정량적 분석을 위해서는 정량한계(LOQ) 이상의 농도 필요
3. 매트릭스에 따라 검출 한계가 달라질 수 있음

## 참고문헌
1. Harris, D.C. (2015). Quantitative Chemical Analysis. W.H. Freeman and Company.
2. Skoog, D.A., West, D.M., Holler, F.J., Crouch, S.R. (2013). Fundamentals of Analytical Chemistry. Cengage Learning.
3. IUPAC. Compendium of Chemical Terminology, 2nd ed. (the "Gold Book"). Compiled by A. D. McNaught and A. Wilkinson. Blackwell Scientific Publications, Oxford (1997).

## 추가 노트
검출 한계는 분석 방법의 성능을 평가하는 중요한 지표지만, 실제 응용에서는 정량한계(LOQ)가 더 중요할 수 있다. 검출 한계 이하의 농도에서는 물질의 존재 여부만 판단 가능하며, 정확한 정량 분석은 어렵다.