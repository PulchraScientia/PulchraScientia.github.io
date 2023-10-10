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
