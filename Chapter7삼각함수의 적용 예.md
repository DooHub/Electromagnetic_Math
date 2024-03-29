
## 예제-1 선전하에 의한 전계

### Z축에 전하($\rho_{L}$)가 있을 때 점 D ($\rho , \phi ,0$)에서의 전기장의 세기는 $\rho$ 방향만 있다.  
![선전하전계](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/0057c34b-0d30-48a0-8bc9-0ed18fdd4b0e)
### $E_{\rho}$ 는 $E_{\rho}=E_{\rho }=\int_{-\infty }^{\infty }\frac{\rho _{L}\rho}{4\pi \varepsilon _{0}(\rho ^{2}+z^{'2})^{\frac{3}{2}}}dz'$ 를 풀어야한다.


### 필요 개념 $1+tan^{2}\alpha =sec^{2}\alpha,\quad sec\alpha = \frac{1}{cos\alpha},\quad \int cos\alpha d\alpha = sin\alpha +C $

 + ### $\int_{-\infty }^{\infty }\frac{\rho _{L}\rho}{4\pi \varepsilon _{0}(\rho ^{2}+z^{'2})^{\frac{3}{2}}}dz'$에서 변수는 z' 이므로 나머지는 상수처리
 + ### $\frac{\rho_{L}\rho}{4\pi \epsilon _{0}}\int _{-\infty }^{\infty }\frac{1}{(\rho ^{2}+z^{'2})^{\frac{3}{2}}}dz'$, 정리 가능하며 $\int _{-\infty }^{\infty }\frac{1}{(\rho ^{2}+z^{'2})^{\frac{3}{2}}}dz'$, 를 A로 보고 A에 대해서 처리
 + 좌표 그림에 따라 z축 위의 임의점 z'은 $z'=\rho tan\alpha$ 나타 낼 수 있고 이를 A에 대입 하여 계산을 진행한다.
 + ### $\rho ^{2}+z^{'2}=\rho ^{2}(1+tan^{2}\alpha)=\rho ^{2}sec^{2}\alpha, \quad dz'=\rho sec^{2}\alpha d\alpha$
 + ### $\frac{1}{(\rho ^{2}+z^{'2})^{\frac{3}{2}}}dz'=\frac{\rho sec^{2}\alpha}{\rho ^{3}sec^{3}\alpha}d\alpha=\frac{1}{\rho ^{2}sec\alpha}d \alpha=\frac{cos \alpha}{\rho ^{2}}d \alpha$
 + ### $\int_{-\infty }^{\infty }dz'$을 $d\alpha$로 변환하면 $-\infty \rightarrow-\frac{\pi}{2},\infty \rightarrow \frac{\pi}{2}$ 된다.
 + ### $A=\int _{-\infty }^{\infty }\frac{1}{(\rho ^{2}+z^{'2})^{\frac{3}{2}}}dz'=\int _{-\frac{\pi}{2}}^{\frac{\pi}{2}}\frac{cos \alpha}{\rho ^{2}}d \alpha =\frac{1}{\rho ^{2}}sin\alpha | _{-\frac{\pi}{2}}^{\frac{\pi}{2}} =\frac{2}{\rho^{2}}$
 + ### $\frac{\rho_{L}\rho}{4\pi \epsilon _{0}}\int _{-\infty }^{\infty }\frac{1}{(\rho ^{2}+z^{'2})^{\frac{3}{2}}}dz'=\frac{\rho _{L}\rho}{4\pi \epsilon _{0}}\frac{2}{\rho^{2}}=\frac{\rho _{L}\rho}{2\phi \epsilon _{0}}$



## 예제-2 면전하에 의한 전계

### y평편에 면전하가 있을 때 점 P에서의 전기장의 세기는 x 방항만 있다. 
### 미소면적 dy'(연두색 선 사이)에서 점P에서의 세기를 구하고 이 미소먼적을 y축의따라 이동하면서 점P에 인가 되는 전기장의 합을 구한다. 
![면전하](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/17794d05-c639-4d8b-bd7d-3ba169302469)

### $E_{x}$는 $E_{x} = \frac{\rho_{s}x}{2\pi \epsilon_{0}}\int _{-\infty}^{\infty}\frac{1}{x^{2}+y'^{2}}dy'$을 풀어야한다.
### Y축의 A와c 사이를 y'라 하고 점(A,P,C)을 연결할 때 사이각을 $\theta$라고 한다. 

+ ### $y'=xtan\theta, \quad x^{2}+y'{2}=x^{2}(1+tan^{2}\theta)=x^{2}sec^{2},\quad dy'=xsec^{2}\theta$ 된다.
+ ### 예제-1과 같이 y'에 대한 변수를 $\theta$로 변환 하면 $-\infty \rightarrow-\frac{\pi}{2},\infty \rightarrow \frac{\pi}{2}$
+ ### $E_{x} = \frac{\rho_{s}x}{2\pi \epsilon_{0}}\int_{-\infty}^{\infty}\frac{1}{x^{2}+y'^{2}}dy'=\frac{\rho_{s}x}{2\pi \epsilon_{0}}\int_{-\pi}^{\pi}\frac{xsec^{2}}{x^{2}sec^{2}}d \theta=\frac{\rho_{s}}{2\pi \epsilon_{0}}\int _{-\pi}^{\pi}d \theta=\frac{\rho _{s}}{2 \epsilon _{0}}$


## 예제-3 발산(divergence)
### 구좌표계에서 $\vec{D}=2rsin\theta cos\phi\hat{a} _{r}+rcos\theta cos\phi \hat{a} _{\theta}-rsin\phi \hat{a} _{\phi}$
![구좌표](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/7a71e37a-e57a-41d5-a747-30fb618ed1c1)
### $\triangledown \cdot \vec{D}=\frac{1}{r^{2}}\frac{\partial }{\partial r}(r^{2}D_{r})+\frac{1}{rsin\theta}\frac{\partial }{\partial \theta}(sin\theta D_{\theta})+\frac{1}{rsin\theta}\frac{\partial D_{\phi}}{\partial \phi}$
### 여기서 $\frac{\partial }{\partial \theta}(sin\theta D_{\theta})$ 를 계산해 보자
### 필요 개념 $sin(a+b)=sin(a)cos(b)+sin(b)cos(a),\quad cos(a+b)=cos(a)cos(b)-sin(a)sin(b)$
+ ### $D_{\theta}=rcos\theta cos\phi, \quad \frac{\partial }{\partial \theta}(sin\theta D_{\theta})= \frac{\partial }{\partial \theta}(sin\theta rcos\theta cos\phi)=r cos\phi \frac{\partial }{\partial \theta}(sin\theta cos\theta)=r cos\phi \frac{\partial }{\partial \theta}(\frac{sin 2\theta}{2})$
+ ### $\frac{\partial }{\partial \theta}(\frac{sin 2\theta}{2})=\frac{2cos 2\theta}{2}=cos 2\theta=cos^{2}\theta-sin^{2}\theta$

## 예제-4 발산(divergence)
### 구좌표계에서 $\vec{D}=sin\theta sin\phi\hat{a} _{r}+cos\theta sin\phi \hat{a} _{\theta}-cos\phi \hat{a} _{\phi}$ 로 주어졌다.
### $\triangledown \cdot \vec{D}=\frac{1}{r^{2}}\frac{\partial }{\partial r}(r^{2}D_{r})+\frac{1}{rsin\theta}\frac{\partial }{\partial \theta}(sin\theta D_{\theta})+\frac{1}{rsin\theta}\frac{\partial D_{\phi}}{\partial \phi}=0$ 가 0이 됨을 보여라 

+ ### $\frac{\partial }{\partial r}(r^{2}D_{r})=\frac{\partial }{\partial r}(r^{2}sin\theta sin\phi\)=2rsin\theta sin\phi\$ ---- 1)
+ ### $\frac{\partial }{\partial \theta}(sin\theta D_{\theta})=\frac{\partial }{\partial \theta}(sin\theta cos \theta sin \phi)=sin \phi(cos^{2}\theta-sin^{2}\theta)$ ----2)
+ ### $\frac{\partial D_{\phi}}{\partial \phi}=\frac{\partial cos \phi}{\partial \phi}=sin \phi$  ---- 3)
+ ### 1),2)와 3)을 적용 하면 $\triangledown \cdot \vec{D}=\frac{1}{r^{2}}(2rsin\theta sin\phi\)+\frac{1}{rsin\theta}sin \phi(cos^{2}\theta-sin^{2}\theta)+\frac{1}{rsin\theta}sin \phi$
+ ### $\triangledown \cdot \vec{D}=\frac{sin \phi}{r}[2sin \theta +\frac{1}{sin \theta}(cos^{2}\theta-sin^{2}\theta)-\frac{1}{sin \theta}]=\frac{sin \phi}{r}\frac{2sin^{2}\theta+cos^{2}\theta-sin^{2}\theta -1 }{sin \theta}$
+ ### $cos^{2}\theta=1-sin^{2}\theta$을 적용 하면, $2sin^{2}\theta+cos^{2}\theta-sin^{2}\theta -1=2sin^{2}\theta+1-sin^{2}\theta-sin^{2}\theta-1=0$
+ ### $\triangledown \cdot \vec{D}=\frac{sin \phi}{r}[0]=0$
+ 
## 예제-5 전기장이 가진 에너지
### 전기자이 가진 에너지를 푸는 과정에 $W_{E}=\frac{\varepsilon _{o}}{2}\int _{2\times10^{-3} }^{3\times10^{-3}}\frac{1}{r^{4}}\int _{0^{\circ}}^{90^{\circ}}(600^{2}cos^{2}\theta +300^{2}sin^{2}\theta)sin \theta d \theta\int _{0}^{\frac{\pi }{2}}d \phi$ 를 폴어야 한다.
### 이중 $B\equiv \int_{0^{\circ}}^{90^{\circ}}(600^{2}cos^{2}\theta+300^{2}sin^{2}\theta)sin\theta d \theta$ 를 계산하라
+ ### $\int_{0^{\circ}}^{90^{\circ}}(600^{2}cos^{2}\theta+300^{2}sin^{2}\theta)sin\theta d \theta =600^{2}\int_{0^{\circ}}^{90^{\circ}}cos^{2}\theta sin \theta d \theta+300^{2}\int_{0^{\circ}}^{90^{\circ}}sin^{2}\theta sin\theta d \theta$
+ ### $u=cos\theta, du=-sin\theta d \theta, \quad \theta=0^{\circ}\rightarrow u=1,\theta=90^{\circ}\rightarrow u=0$
+ ### u에 대해 재 정리 하면
+ ### $600^{2}\int_{0^{\circ}}^{90^{\circ}}cos^{2}\theta sin \theta d \theta=600^{2}\int_{1}^{0}-u^{2}du=600^{2}\int_{0}^{1}u^{2}du=600^{2}\frac{1}{3}u^{3}|_{0}^{1}=\frac{600^{2}}{3}$    ---1)
+ ### $300^{2}\int_{0^{\circ}}^{90^{\circ}}sin^{2}\theta sin\theta d \theta=300^{2}\int_{0^{\circ}}^{90^{\circ}}(1-cos^{2}\theta) sin\theta d \theta=300^{2}\int_{0^{\circ}}^{90^{\circ}} sin \theta d \theta -300^{2}\int_{0^{\circ}}^{90^{\circ}}cos^{2}\theta sin\theta d \theta$
+ ### $300^{2}\int_{0^{\circ}}^{90^{\circ}} sin \theta d \theta=300^{2}(-cos \theta | _{0^{\circ}}^{90^{\circ}})=300^{2}$
+ ### $-300^{2}\int_{0^{\circ}}^{90^{\circ}}cos^{2}\theta sin\theta d \theta$ 의 경우 1)의 값을 활용 $-\frac{300^{2}}{3}$
+ ### $300^{2}\int_{0^{\circ}}^{90^{\circ}}sin^{2}\theta sin\theta d \theta =\frac{2\times 300^{2}}{3}$
+ ### $\frac{600^{2}}{3} +\frac{2 \times 300^{2}}{3}=180 \times 10^{3}$
