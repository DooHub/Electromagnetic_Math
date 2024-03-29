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
### Q=2C, $\ \vec{E}=y\hat{a}_ {x}+x \hat{a}_ {y}+2\hat{a}_{z}$, 점 A(0.8,0.6,1)점 B(1,0,1) 일 때, 점 B에서 점A로 최단 거리(=직선거리)로 움직일 때 필요한 에너지를 구하라.
### Background
+ ### 자기장에 전하가 존재하면 자기장 방향으로 전하는 힘을 받으며, 이를 이동하기 위해서는 에너지가 필요하다.
<img src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/75a30c3a-0260-4011-89dc-8afbb87eec3b" width="600" />

+ ### $d \vec{L}$의 의미는 직교 좌표에서  x,y,z축의 각 방향으로 미소변위를 말하다.
  ### $d \vec{L}=dx\hat{a}_ {x} +dy\hat{a}_ {y}+dz\hat{a}_{z}$로 표현 할 수 있다.
+ ### dot product의 정의 및 계산
  ### $\vec{A}\cdot \vec{B}=\left| A \right|\left| B \right|\text{cos}\theta$. 적용한 값은 벡터이지만 결과 같은 스칼라가 된다.
  ### m에 $\vec{G}$ 로 힘을 주었을 때, $\vec{G}$ 힘을 받아 이동하다. 이 때의 일의 의미를 dot product 표현 할 수 있다.
  
  <image src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/6d5e120e-a214-4523-bf1b-f623dbf342d4" width="400" />
  
  ### $\hat{a}_x \cdot \hat{a}_x =\text{cos}0^{\circ}=1, \quad \hat{a}_x \cdot \hat{a}_y=\hat{a}_x \cdot \hat{a}_z =\text{cos}90^{\circ}=0$
__________________________________________________________________________________________________________________________________________
### 풀이
  + ### $\vec{E} \cdot d \vec{L}=(y\hat{a}_x+x\hat{a}_y+2\hat{a}_z)\cdot(dx\hat{a}_x+dy\hat{a}_y+dz\hat{a}_z)$
    ### $\qquad \quad=ydx+xdy+2dz$
  + ### $\int_{B}^{A}\vec{E}\cdot d\vec{L}=\int_{(1,0,1)}^{(0.8,0.6,1)}(ydx+xdy+2dz)=\int_{1}^{0.8}ydx+\int_{0}^{0.6}xdy+\int_{1}^{1}2dz, \quad(\int_{a}^{a}f(x)dx=0)$
  + ### $\int_{1}^{0.8}ydx$ 처리 시 y는 상수 처리 하면 안 됨. 두 점 A,B 사이 거리에서 x가 변화면 y도 변함. y를 x에 대한 변수로 변경. (단, x가 변할 때 y가 변하지 않으면 상수 취급 가능)
    ### y=ax+b, A(0.8,0.6,1), B(1,0,1), $a=\frac{0.6-0}{0.8-1}=-3$, B(1,0,1) 대입 0=-3+b, b=3, $\therefore y=-3x+3$
    ### $\int_{1}^{0.8}ydx=\int_{1}^{0.8}(-3x+3)dx=\left[-\frac{3}{2}x^2+3x \right]_{1}^{0.8}=-60\times 10^{-3}$
  + ### $\int_{0}^{0.6}xdy=\int_{0}^{0.6}(\frac{-1}{3}y+1)dy=\left[ -\frac{1}{3}\frac{1}{2}y^2+y \right]_{0}^{0.6}=-540\times 10^{-3}$
  + ### $W=-Q\int_{B}^{A}\vec{E}\cdot d\vec{L}=-2\times 480 \times 10^{-3}$
  + ### 값이 - 의미는 전계의 방향에 역향(+ 양수 값)하는 것이 아니라, 전계의 방향과 동일하게 이동했다고 볼 수 있음.













  
