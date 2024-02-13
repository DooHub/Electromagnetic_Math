## Background-1

### $\lim_{x \to 0} \frac{\text{sin}x}{x}=1$증명하라
+ ### 라디안 : 반지름과 호의 길이의 비, 1 라디안 : 반지름(r) = 호의 길이 (라디안은 비율이기 때문에 원의 크기에 상관없이 적용)
+ ### 원주율($\pi$) : 원의 지름(d)에 대한 둘레(l)의 비율,  $\pi=\frac{\text{l}}{\text{d}}=\frac{\text{l}}{\text{2r}}, 2\pi r=\text{l}$
+ ### 부채꼴의 넓이 : $\frac{1}{2}r^{2}\theta$
+ ### 반지름이 1인 원에서 넓이에 대해 다음이 성립 된다.
![geogebra-export](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/406ad945-29ae-48b5-b646-e0173c8b154c)

  ### 삼각형ABC넓이 < 부채꼴ABD넓이 < 삼각형AED넓이 $\longrightarrow \frac{1}{2}\times 1 \times \text{sin}x\lt \frac{1}{2} \times 1^{2}\times x \lt \frac{1}{2} \times 1 \times \text{tan}x$
  ### $\frac{2}{\text{sin}x}$을 곱해주면 $1\lt \frac{x}{\text{sin}x}\lt \frac{1}{\text{cos}x}$
  ### 1보다 큰수의 역수는 1보다 작고 0보다는 크다. $\quad 1\gt \frac{\text{sin}x}{x}\gt \text{cos}x \gt0, \quad \lim_{x \to 0} \text{cos}x=1\quad \therefore \frac{\text{sin}x}{x}=1$
## Background-2
### $\lim_{x \to 0} \frac{\text{cos}x-1}{x}=0$증명하라
+ ### $\lim_{x \to 0} \frac{\text{cos}x-1}{x}=\lim_{x \to 0} \frac{(\text{cos}x-1)(\text{cos}x+1)}{x(\text{cos}x+1)}=\lim_{x \to 0} \frac{\text{cos}^{2}x-1}{x(\text{cos}x+1)}=\lim_{x \to 0} \frac{-\text{sin}^{2}x}{x(\text{cos}x+1)}$
### $\qquad \qquad \qquad \quad \ =\lim_{x \to 0}\frac{\text{sin}x}{x}\frac{-\text{sin}x}{\text{cos}x+1}, \quad \lim_{x \to 0}\frac{\text{sin}x}{x}=1,\lim_{x \to 0}\frac{-\text{sin}x}{\text{cos}x+1}=\frac{0}{2}=0 \quad \therefore 1 \times \frac{0}{2}=0$

## 증명
+ ### $(\text{sin}x)'=\text{cos}x$
  ### $\qquad \quad=\lim_{h \to 0} \frac{\text{sin}(x+h)-\text{sin}x}{h}=\lim_{h \to 0} \frac{\text{sin}x\text{cos}h+\text{sin}h\text{cos}x-\text{sin}x}{h}=\lim_{h \to 0} \frac{\text{sin}x(\text{cos}h-1)+\text{sin}h\text{cos}x}{h}$
  ### $\qquad \qquad \lim_{h \to 0} \frac{\text{sin}x(\text{cos}h-1)}{h}=0,\lim_{h \to 0} \frac{\text{sin}h\text{cos}x}{h}=1\times \text{cos}x$
  
+ ### $(\text{cos}x)'=-\text{sin}x$
  ### $\qquad \quad=\lim_{h \to 0} \frac{\text{cos}(x+h)-\text{cos}x}{h}=\lim_{h \to 0} \frac{\text{cos}x\text{cos}h-\text{sin}h\text{sin}x-\text{cos}x}{h}=\lim_{h \to 0} \frac{\text{cos}x(\text{cos}h-1)-\text{sin}h\text{sin}x}{h}$
  ### $\qquad \qquad \lim_{h \to 0} \frac{\text{cos}x(\text{cos}h-1)}{h}=0,\lim_{h \to 0} \frac{\text{sin}h\text{sin}x}{h}=-1\times \text{sin}x$

+ ### $(\text{tan}x)'=-\text{sec}^{2}x$
  ### $\qquad \quad=(\frac{\text{sin}x}{\text{cos}x})'=\frac{\text{cos}x\text{cos}x+\text{sin}x\text{sin}x}{\text{cos}^{2}x}=\frac{1}{\text{cos}^{2}x}=\text{sec}^{2}x$

## 응용문제-1
### 전속밀도가 $\overrightarrow{D}=e^{-x}\text{sin}y\hat{a_{x}}-e^{-x}\text{cos}y\hat{a_{y}}+2z\hat{a_{z}}\ \text{C}/m^{2}$으로 주어졌다.
### 원점에서 $\bigtriangleup v =10^{-9}m^{3}$에 둘러싸인 총 전하량의 근사치는 $\text{Q}=(\frac{\partial D_{x}}{\partial x}+\frac{\partial D_{y}}{\partial y}+\frac{\partial D_{z}}{\partial z})|_{(0,0,0)}\bigtriangleup v$이다. $\text{Q}$를 구하여라
+ ### $\frac{\partial D_{x}}{\partial x}=\frac{\partial }{\partial x}(-e^{-x}\text{sin}y)=\text{sin}y\frac{d }{dx}(-e^{-x})=-e^{-x}\text{sin}y$
+ ### $\frac{\partial D_{y}}{\partial y}=\frac{\partial }{\partial y}(-e^{-x}\text{cos}y)=-e^{-x}\frac{d }{dy}(\text{cos}y)=e^{-x}\text{sin}y$
+ ### $\frac{\partial D_{z}}{\partial z}=\frac{\partial }{\partial z}(2z)=2\frac{d }{dz}(z)=2$
+ ### $\text{Q}=(-e^{-x}\text{sin}y+e^{-x}\text{sin}y+2)|_{(0,0,0)}\bigtriangleup v=2\times 10^{-9}\text{C}$ -단위 주

## 가우스법칙
### 전속밀도 $\text{D}$ $(C/m^{2})$는 단위면적당 전속의 수를 전속밀도라 한다.
### 표면의 전속밀도의 면적분은 면 내의 총 전하량과 같다.-폐곡면 내 $\text{Q}=\oint_{s}^{}\textbf{D}\bullet d\textbf{S}$
### 전속밀도 $(C/m^{2}$) 와 전계($V/m$)의 관계 $\quad \Longrightarrow \text{D}=\varepsilon_{0}\textbf{E}$


## 응용문제-2
### 체적전하밀도 $\rho_{v}$는 전속밀도 $\overrightarrow{D}$ 로부터 $\rho_{v}=\nabla \cdot \overrightarrow{D}$ 의 관계로 구해진다. 원통좌표계에서 $\nabla \cdot \overrightarrow{D}$ 는 다음과 같다.
### $\qquad  \qquad \nabla \cdot \overrightarrow{D}=\frac{1}{\rho}\frac{\partial }{\partial \rho}(\rho D_{\rho})+\frac{1}{\rho}\frac{\partial D_{\phi}}{\partial \phi}+\frac{\partial D_{z}}{\partial z}$
### 점 $P(\rho=2,\phi=110^{\circ },z=1)$ 에서 $\rho_{v}$ 를 구하여라.
### 전속밀도는 다음과 같다. $\overrightarrow{D}=2\rho z^{2}\text{sin}^{2}\phi \hat{a}_{\rho}+\rho z^{2}\text{sin}2 \phi \hat{a}_{\phi}+2 \rho^{2} \text{sin}^{2} \phi \hat{a}_{z} \ C/m^{2}$
