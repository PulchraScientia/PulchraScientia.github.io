---
published: true
layout: single
title: "Gradient Descent"
---

## 기울기
$$\frac{\Delta y}{\Delta x} = \frac{y_ 2 - y_ 1}{x_ 2 - x_ 1}$$

## 극한(무한소)과 미분
$$y = f(x)$$   

$$\frac{dy}{dx}= lim_ {\substack h \to 0}\frac{f(x+h)-f(x)}{(x+h) - x} $$

## 도함수
$$g(x) - \lim_ {h \to 0}\frac{f(x+h) = f(x)}{(x+h)-x}$$   

$$y\prime = f\prime(x) = g(x)$$

## 함성함수 미분
$$y = f \circ g(x) = f(g(x))$$   

$$y\prime = f\prime(g(x)) \cdot g\prime(x)$$   

$$y = f(h), h = g(x)$$   

$$chain \quad rule \quad!$$   

$$\frac{dy}{dx} = \frac{df}{dh} \cdot \frac{dh}{dx} = f\prime(h) \cdot (\frac{d}{dx}g(x)) = f\prime(g(x)) \cdot g\prime(x)$$

## 편미분
### 다변수 함수
* 여러개의 변수를 입력으로 받는 함수
* z = f(x, y)
### 편미분이란
* 다변수 x, y를 입력으로 받는 함수 f를 x로 미분할 경우, 하나의 변수를 남겨놓고 나머지를 상수 취급
* 함수 f를 x변수(축)으로 미분
$$\frac{\partial f}{\partial x} = \lim_ {h \to 0} \frac{f(x+h, y) - f(x, y)}{(x+h)-x}$$
* y값에 대해 뚝 잘랐을때, x축에 대한 기울기

## 함수의 입출력 형태
* 함수의 입력이 백터인 경우
* 함수의 출력이 벡터인 경우
* 함수의 입력이 행렬인 경우
* 함수의 출력이 행렬인 경우
* 입력과 출력이 백터인 경우
$$\begin{equation*}
  y = 
  \begin{bmatrix} 
  y_ 1 \\
  \vdots \\
  y_ m
  \end{bmatrix} 
\end{equation*}$$

  $$\begin{equation*} y = \begin{bmatrix} y_1 \\ \vdots \\  y_m \end{bmatrix} = f(x) = f(\begin{bmatrix} x_1 \\ \vdots \\ x_n \end{bmatrix}), \quad where f: \mathbb R^n \to \mathbb R^m \end{equation*}$$

## 스칼라를 벡터로, 스칼라를 행렬로 미분
 * 미분 결과는 gradient 벡터가 되어 방향과 크기를 모두 나타냄
 * $\nebula $

## 벡터를 스칼라로, 벡터를 벡터로 미분

?


* Loss 값을 최소로하는 Loss Function의 입력값 $\theta$ 를 찾자.
* Gradient Descent : x로 미분한 기울기를 활용하여 좀 더 낮은 곳으로 점차 나아가자

* Global and Local Minima
  * 국소점에 빠진다면?
* Loss Minimization using Gradient Descent
  * 1D 케이스를 높은 차원의 $\theta$ 로 확장
  * 모든 차원에서 동시에 local minima가 되기 어려우므로, 대체로 global minima에ㅐ 근접할 수 있다. 


