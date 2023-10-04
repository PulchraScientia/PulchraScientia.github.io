---
published: true
layout: single
title: "Loss Function : Mean Square Error"
---
* 데이터를 넣었을때 출력을 반환하는 가상의 함수를 모사하는것
* Linear Layer 함수를 통해 원하는 함수를 모사해보자
  * Linear Layer 함수가 얼마나 원하는만큼 동작하는지 측정
  * 잘 동작하는지, 수치화
## Loss
* Loss ( 손실값 : 원하는 출력값(target, y)와 실제 출력값( output, y) 차이의 합
* Loss 가 작을수록 가상의 함수를 잘 모사한 것
* Loss가 작은 Linear Layer를 선택

$$Loss \quad = \quad \sum^{N} _ {i=1} ||y_i - \hat{y_i}||$$   
$$\quad = \quad \sum^{N}_{i=1} ||y_i - f(x_i)||$$
참고: $||x|| = \sqrt{x^2}$ 

### Loss Function
* Linear Layer의 파라미터를 바꿀때마다 Loss를 계산
* Loss Function
    * 입력 : Linear Layer의 파라미터
    * 출력 : Loss

$$L(\theta) = \sum^{N}_{i=1}||y_i - f _ {\theta}{x_i}||,$$   
$$where \quad \theta = {W, b}.$$

### Euclidean Distance
* 두 점 사리의 거리
$$||y - \hat{y}||_2 = \sqrt{()^2 + \dots + ()^2,}$$
