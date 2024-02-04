
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
