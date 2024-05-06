## 유리함수,분수함수,다항함수
### $f(x)=\frac{x}{(x+1)^3}, \quad g(x)=\frac{2x+2}{x^2-4x+8}, \quad h(x)=\frac{x^5-x+1}{x^3+5x}$


등과 같이 두개의 다항의 분수형태로 된 함수를 분수함수라고 하고 특히, 분모가 상수일 때를 다항함수라고 한다.  

분수함수와 다항함수를 합쳐서 유리함수라고 한다.  

## 분수함수의 적분법
### 1)분자의 차수가 분모의 차수보다 작으면 -->치환적분법이나 로그함수를 생각해 본다.
### 2)분자의 차수가 분모의 차수보다 크면:  
###   -몫과 나머지를 구한다. 몫: 다항함수, 나머지:분자가 분모보다 차수가 작은 분수 함수  
###   - 분자가 분모보다 차수가 작은 분수함수들의 합으로 만든다.

-----------------------------------------------------------------------------

### 예제1 - 부정적분 $I=\int_{}^{}\frac{x+1}{x^2-2x+2}dx$를 구하여라
$I=\int_{}^{}\frac{x+1}{(x-1)^2+1}dx, \quad (u=x-1,du=dx) \quad, I=\int_{}^{}\frac{u+2}{u^2+1}du=\int_{}^{}\frac{u}{u^2+1}du+\int_{}^{}\frac{2}{u^2+1}du$  
$\int_{}^{}\frac{u}{u^2+1}du=\frac{1}{2}ln\left| u^2+1 \right|+C_{1}=\frac{1}{2}ln\left| x^2-2x+2 \right|+C_{1}$  
$\int_{}^{}\frac{2}{u^2+1}du=\int_{}^{}\frac{2\text{sec}^2\theta}{\text{tan}^2\theta+1}d\theta=2\theta+C_{2}=2\text{tan}^{-1}u+C_{2}=2\text{tan}^{-1}(x-1)+C_{2},\quad(u=\text{tan}\theta,du=\text{sec}^2\theta d\theta,\text{tan}^2\theta+1=\text{sec}^2\theta)$  
$I=\frac{1}{2}ln\left| x^2-2x+2 \right|+C_{1}+2\text{tan}^{-1}(x-1)+C_{2}=\frac{1}{2}ln\left| x^2-2x+2 \right|+2\text{tan}^{-1}(x-1)+C$  

### 예제2 - 부정적분 $I=\int_{}^{}\frac{3x+1}{x^2-x-6}dx$를 구하여라
