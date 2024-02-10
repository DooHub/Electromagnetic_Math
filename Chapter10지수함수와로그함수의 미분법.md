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
