## 두 함수 y=g(u),u=f(x)에 대하여 f 와 g의 합성함수 $g \circ f$ 는 $(g \circ f)(x)=g(f(x))$로 정의 한다.
## 두 함수 y=g(u),u=f(x)가 미분 가능할 때, 합성함수 $y=(g \circ f)(x)=g(f(x))$도 미분가능하고, 그 도함수는 다음과 같다.
## $\frac{dy}{dx}=\frac{dy}{du}\frac{du}{dx}$ 이를 합성함수의 미분버 또는 연쇄법칙(Chain rule)이라고 한다.

### 예제-1 $u=x^{2}+1$ 이고 $y=u^{2}+3u+1$ 일 때, $\frac{dy}{dx}$ 을 구하여라
+ ### $\frac{dy}{dx}=\frac{dy}{du}\frac{du}{dx}$
+ ### $\frac{dy}{du} =2u+3=2(x^{2}+1)+3, \quad \frac{du}{dx}=2x$
+ ### $\frac{dy}{du}\frac{du}{dx}=(2x^{2}+5)2x=4x^{2}+10x$

## 다항함수의 제곱승을 미분 하는 방법
### $\frac{d}{dx}{f(x)}^{n}=n{f(x)}^{n-1}f(x)'$
### (증명) 
### $y=u^{n}, u=f(x)$라 하면 $\frac{dy}{dx}=\frac{dy}{du}\frac{du}{dx}=nu^{n-1}f(x)'=nf(x)^{n-1}f(x)'$
### 예제-2 $y=cos(x^{2}+1)$ 를 미분하라
+ ### $y=-2xsin(x^{2}+1)$
