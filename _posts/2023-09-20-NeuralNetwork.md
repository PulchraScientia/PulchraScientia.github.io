---
published: true
layout: single
title: "Neural Network"
---

## Matrix Multiplication
* 행렬 곱
* inner Product, Dot Product

$$\begin{equation*} 
  A \cdot B =
    \begin{bmatrix}
    1 & 2 & 3 \\ 
    4 & 5 & 6
    \end{bmatrix}
  \cdot
    \begin{bmatrix} 
    1 & 2 \\
    3 & 4 \\ 
    5 & 6
  \end{bmatrix}
  \end{equation*}$$

n by h matrix가 N개 쌓여있다고 볼 수 있음. 
$$(N, n, h) \times (N, h, m) = (N, n, m)$$ 

## Linear Layer
* 신경망의 가장 기본 구성 요소
* Fully-connected Layer
* 내부 가중치 파라미터(weight parameter)에 따른 선형 변환을 수행하는 함수 = W, b

### 작동방식
* 각 입력 노드들에 wieght를 곱하고, 모두 합친 뒤 bias를 더하면 출력노드 값을 얻을 수 있다.
* 이 파라미터를 잘 조절하여 주어진 입력에 대하여 원하는 출력을 만들 수 있다.
### Equation
* 행렬곱
* n차원에서 m차원으로의 선형 변환함수
* $x \in \mathbb R ^{k \times n} \quad W \in \mathbb R ^{n \times m}$ $\implies$ $y \in \mathbb R^{k \times m}$
$$y = f(x) = x \cdot W + b$$

* x를 미니배치에 관계없이 단순히 벡터로 볼 경우
  * (m, n) X (n, 1) = (m, 1)
$$y = f(x) = W^{T} \cdot + b,$$
$$where x \in \mathbb R ^{n}, W ^{T} \in \mathbb R^{m \times n}, b \in \mathbb R ^{m} \quad and \quad y \in \mathbb R ^{m}$$

* x를 미니배치 (N개) tensor로 표현할경우
  * (N, n) X (n, m) = (N, m)
$$y = f(x) = x \cdot W + b,$$
$$where x \in \mathbb R ^{N \times n}, W \in \mathbb R ^{n \times m}, b \in \mathbb R ^{m} \quad and \quad y \in \mathbb R ^{N \times n}$$
