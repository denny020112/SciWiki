---
aliases:
  - 그라디언트 연산자
  - 나블라 연산자
category:
  - 벡터 미적분학
  - 미분 연산자
related_concepts:
  - 기울기
  - 발산
  - 회전
  - 라플라스 연산자
tags:
  - 수학
  - 벡터
  - 해석
  - 물리
  - 미적분학
---

```table-of-contents
title: 
style: nestedList # TOC style (nestedList|nestedOrderedList|inlineFirstLevel)
minLevel: 0 # Include headings from the specified level
maxLevel: 0 # Include headings up to the specified level
includeLinks: true # Make headings clickable
debugInConsole: false # Print debug info in Obsidian console
```
# 델 연산자 (∇)

## 정의
델 연산자(∇; Del operator)는 벡터 미적분학에서 사용되는 미분 [[Operator|연산자]]로, [[Partial Differentiation|편미분]] 연산자들의 벡터다. 나블라 (Nabla)라고도 표현한다. 

## 수학적 표현
3차원 직교좌표계에서 델 연산자는 다음과 같이 표현된다:

$$\nabla = \frac{\partial}{\partial x}\hat{i} + \frac{\partial}{\partial y}\hat{j} + \frac{\partial}{\partial z}\hat{k}$$

여기서 $\hat{i}$, $\hat{j}$, $\hat{k}$는 x, y, z 방향의 단위벡터다.

## 연산
### 기울기(Gradient)
스칼라장 $f$에 대해,
   $$\nabla f = \frac{\partial f}{\partial x}\hat{i} + \frac{\partial f}{\partial y}\hat{j} + \frac{\partial f}{\partial z}\hat{k}$$

스칼라장에서 가장 빠르게 증가하는 방향과 크기를 나타낸다.[^1]
	![[del gradient.png|400]]
	
### 발산(Divergence)
벡터장 $\mathbf{F} = F_x\hat{i} + F_y\hat{j} + F_z\hat{k}$에 대해,
   $$\nabla \cdot \mathbf{F} = \frac{\partial F_x}{\partial x} + \frac{\partial F_y}{\partial y} + \frac{\partial F_z}{\partial z}$$
벡터장의 발산 정도를 나타낸다. [^2]
	![[del divergence.png|400]]
### 회전(Curl)
벡터장 $\mathbf{F}$에 대해,
   $$\nabla \times \mathbf{F} = \left(\frac{\partial F_z}{\partial y} - \frac{\partial F_y}{\partial z}\right)\hat{i} + \left(\frac{\partial F_x}{\partial z} - \frac{\partial F_z}{\partial x}\right)\hat{j} + \left(\frac{\partial F_y}{\partial x} - \frac{\partial F_x}{\partial y}\right)\hat{k}$$

벡터장의 회전 정도를 나타낸다. [^3]
	![[del curl.png|400]]



## 시각화
간단한 3차원 좌표계와 델 연산자 표현:

- 붉은 화살표가 각 지점에서의 화살표를 나타낸다


[^1]: 붉은 화살표가 각 지점에서의 기울기를 나타낸다.
[^2]: 벡터장 F = (x, y)의 발산 (검은색)
[^3]: 벡터장 F = (-y, x)의 회전 (검은색)