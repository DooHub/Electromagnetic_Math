## 용어 정의
### 원시함수, 부정적분(Indefinite integral), 적분한다, 적분법
### $y=x^{3}$을 미분하면 $y'=3x^{2}$ 이다. 이를 역으로 생각하면 $3x^{2}$  을 도함수로 갖는 함수는  $x^{3}$이다.
+ ### 도함수를 알 때 미분하기 전 원래의 함수를 원시함수 또는 부정적분이라고 한다.
+ ### 부정적분을 구하는 것을 적분한다고 한다.
+ ### 부정적분을 구하는 방법을 적분법이라고 한다.

## 적분의 표현
### 일반적인 원시함수(부정적분)은 상수 C를 써서 나타내어야 한다.
+ ### $3x^{2}$의  부정적분은 $x^{3}+\text{C}$ 이다.
+ ### 이를 다음과 같이 표현 한다. $\int_{}^{}3x^{2}dx = x^{3}+\text{C}$
### 상기 내용을 일반화하여 나타내면 다음과 같다. 
+ ### $\int_{}^{}f(x)dx = F(x)+\text{C}$
  + ### f(x): 피적분함수
  + ### F(x): 부정적분(원시함수)
  + ### x :적분 변수
  + ### C :적분 상수

## 일반화 증명 $\int_{}^{}x^{n}dx =\frac{1}{n+1}x^{n+1}+\text{C}$
+ ### $(x^{n})'=nx^{n-1},\quad  n\longrightarrow n+1, \quad (x^{n+1})'=(n+1)x^{n}$
+ ### $(x^{n+1})'=(n+1)x^{n}, \quad \frac{1}{n+1}(x^{n+1})'=x^{n}$
+ ### $\int_{}^{}x^{n}dx =\frac{1}{n+1}x^{n+1}+\text{C}$

## 부정적분의 기본 공식 (단, k는 상수)
+ ### $\int_{}^{}kdx =kx+\text{C}$
+ ### $\int_{}^{}kf(x)dx =k\int_{}^{}f(x)dx$
+ ### $\int_{}^{}(f(x)+g(x))dx =\int_{}^{}f(x)dx+\int_{}^{}g(x)dx$
+ ### $\int_{}^{}(ax+b)^{n}dx =\frac{1}{a(n+1)}(ax+b)^{n+1}+\text{C} (a \ne 0, n\ne 1)$
  + ### Chain rule  $\ u=ax+b, \quad du=adx \longrightarrow \int_{}^{}(ax+b)^{n}dx=\int_{}^{}\frac{1}{a}u^{n}du=\frac{1}{a(n+1)}(ax+b)^{n+1}+\text{C}$

## 응용예제
### 전하 Q가 전기장 $\overrightarrow{E}$내에서 점 B로 부터 점 A로 이동하는데 들어가는 에너지는 $\text{W}=-Q\int_{B}^{A}\overrightarrow{E}\cdot d\overrightarrow{L}$나타난다.
### Q=2C, $\ \overrightarrow{E}=y\hat{a}_{x}+x\hat{a}_{y}+2\hat{a}_{z}$, 점 A(0.8,0.6,1)점 B(1,0,1) 일 때, 점 B에서 점A로 최단 거리로 움직일 때 필요한 에너지를 구하라.
### Background
+ ### 자기장에 전하가 존재하면 자기장 방향으로 전하는 힘을 받는다.
<img src="" width="300" />
