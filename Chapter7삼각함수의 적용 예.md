
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
