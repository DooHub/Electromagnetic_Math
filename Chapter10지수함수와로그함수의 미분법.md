## 증명 1
### $\lim_{x\rightarrow 0}(1+x)^{\frac{1}{x}}=e$를 이용하여 y=lnx의 도함수를 구해보자.
### $(lnx)'=\frac{1}{x}$의 증명
+ ### $(lnx)'=\lim_{h\rightarrow 0}\frac{ln(x+h)-ln(x)}{h}=\lim_{h\rightarrow 0}\frac{1}{h}ln(\frac{x+h}{x})$
### $\qquad \qquad \   =\lim_{h\rightarrow 0}\frac{x}{h}\frac{1}{x}ln(1+\frac{h}{x})=\frac{1}{x}\lim_{h\rightarrow 0}ln(1+\frac{h}{x})^{\frac{x}{h}}, \qquad Let \ \frac{h}{x}=a, \quad \lim_{h\rightarrow 0}ln(1+\frac{h}{x})^{\frac{x}{h}}=ln\lim_{a\rightarrow 0}(1+a)^{\frac{1}{a}}=lne$
### $\qquad \qquad \   =\frac{1}{x}\lim_{h\rightarrow 0}ln(1+\frac{h}{x})^{\frac{x}{h}}=\frac{1}{x}ln{e}=\frac{1}{x}$

## 증명 2
### $(lnx)'=\frac{1}{x}$을 이용하여 $y=log_{a}x(a>0,a\neq 1)$ 도함수를 구해 보자
### $(log_{a}x)'=\frac{1}{xlna}$의 증명
+ ### $(log_{a}x)'=(\frac{lnx}{lna})'=\frac{1}{lna}(lnx)'=\frac{1}{xlna}, \qquad log_{a}b=\frac{log_{c}b}{log_{c}a}$

## 예제-1
### $y=ln2x$을 미분 하라
+ ### Method 1 $y'=(ln2x)'= (ln2 +lnx)'=(lnx)'=\frac{1}{x}$
+ ### Method 2 $Let \ d=2x, d'=2, (lnu)'=\frac{1}{u}, \quad \therefore y'=2\frac{1}{2x}=\frac{1}{x}$

## 예제-2
### $y=x^{lnx},(x>0)$을 미분 하라
+ ### $lny=lnx^{lnx}=lnxlnx=(lnx)^{2}, \quad \frac{d(lny)}{dy} \frac{dy}{dx}=2lnx\frac{1}{x}, \quad \frac{d(lny)}{dy}=\frac{1}{y}$
+ ### $\frac{d(lny)}{dy} \frac{dy}{dx}= \frac{1}{y}\frac{dy}{dx}=2lnx\frac{1}{x},\quad \frac{dy}{dx}=y2lnx\frac{1}{x}=2x^{lnx-1}lnx $


## 증명 3
### 자연로그의 미분법을 이용하여 지수함수 $y=a^{x}$ 도함수를 구해 보자
### $(a^{x})'=a^{x}lna \ (a>0, a\neq 1)$ 증명
+ ### $lny=lna^{x}=xlna, \quad \frac{d(lny)}{dy}\frac{dy}{dx}=(xlna)'=lna, \frac{1}{y}\frac{dx}{dy}=lna, \frac{dx}{dy}=ylna =a^{x}lna$

## 증명 4
### $(a^{x})'=a^{x}lna (a>0, a\neq 1)$을 이용하여 $(e^{x})'=e^{x}$ 임을 보이자.
+ ### $(a^{x})'=a^{x}lna, \ a \to e, \quad (e^{x})'=e^{x}lne=e^{x}$ 

## 응용문제
### $\triangledown \times \vec{E} = -\frac{\partial \vec{B}}{\partial t}$는 맥스웰의 네 개 방정식 중의 하나이다. 원통좌표계에서 축방향(z방향)의  
### 자기장의 시간변화에 의해 축 주위를 도는 전기장이 만들어진다. 이 부분을 다시 쓰면 다음과 같다.
### $(\triangledown \times\vec{E}) _{z}=\frac{1}{ \rho} \frac{\partial (\rho E _{\phi})}{\partial \rho}=-\frac{\partial B _{z}}{\partial t}$
### 자기장은 다음과 같다.
### $B_{z}=B_{0}e^{kt}$
### $E_{\phi}$를 구하여라. 단, 적분과정에서 적분상수는 0이다.
![cynder](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/c198bc90-22d1-4949-919c-6d4b6d4b10bb)

+ ### $-\frac{\partial B_{z}}{\partial t}=-\frac{\partial B_{0}e^{kt}}{\partial t}=-B_{0}\frac{\partial e^{kt}}{\partial t}=-B_{0}ke^{kt}$
