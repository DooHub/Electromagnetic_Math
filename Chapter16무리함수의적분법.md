## 1. 피적분함수가 무리함수를 포함하는 경우  
###   무리함수를 적분하는 기본적인 방법은 제곱근 기호를 없애는 것이다.
<img src= "https://github.com/DooHub/Electromagnetic_Math/assets/99073912/e4301a91-42a3-482c-9865-d742bfef8443" width=600 />


### 예제-1 부정적분 $I=\int_{}^{}\frac{1}{2x+\sqrt{x}}dx$를 구하여라.
### $Let \quad u=\sqrt{x}=x^{\frac{1}{2}},du=\frac{1}{2}x^{-\frac{1}{2}}dx=\frac{1}{2\sqrt{x}}dx,2udu=dx$
### $I=\int_{}^{}\frac{2u}{2u^2-u}du=\int_{}^{}\frac{2}{2u-1}du=ln\left| 2u \right|+C=ln\left| 2\sqrt{x} \right|+C,\ (\int_{}^{}\frac{1}{ax+b}dx=\frac{1}{a}ln\left| ax+b \right|+C)$


### 예제-2 부정적분  $I=\int_{}^{}x\sqrt[3]{x-2}dx$를 구하여라.
+ ### $Let \quad u=x-2,du=dx \quad I=\int_{}^{}(u+2)u^{\frac{1}{3}}du=\int_{}^{}(u^{\frac{4}{3}}+2u^{\frac{1}{3}})du=\frac{3}{7}u^{\frac{7}{3}}+2\frac{3}{4}u^{\frac{4}{3}}+C$
  ### $I=\frac{3}{7}(x-2)^{\frac{7}{3}}+\frac{3}{2}(x-2)^{\frac{4}{3}}+C$

### 예제-3 부정적분  $I=\int_{}^{}\sqrt{a^2-x^2}dx$를 구하여라.
+ ### 상기 방식으로는 접근이 어려움. 삼각함수를 고려하여 계산, 항의 제곱 형태
  ### $Let \quad x=a\text{sin}\theta,dx=a\text{cos}\theta d \theta, \quad I=\int_{}^{}\sqrt{a^2-a^2\text{sin}^2\theta}a\text{cos}\theta d \theta =\int_{}^{}\sqrt{a^2\text{cos}^2\theta}a\text{cos}\theta d \theta=\int_{}^{}a^2\text{cos}^2\theta d \theta=a^2\int_{}^{}\text{cos}^2\theta d \theta$
  ### 제곱형태의 삼각함수를 제곱이 아닌 형태로 변경 $\text{cos}(\alpha+\beta)=\text{cos}\alpha\text{cos}\beta-\text{sin}\alpha\text{sin}\beta \ ,\text{sin}^2\alpha=1-\text{cos}^2\alpha$
  ### $I=a^2\int_{}^{}\text{cos}^2\theta d \theta=a^2\int_{}^{}\frac{1+\text{cos}2\theta}{2}d \theta=\frac{a^2}{2}\left[ \theta +\frac{1}{2}\text{sin}2\theta \right]+C=\frac{1}{2}a^2\text{sin}^{-1}\frac{x}{a}+\frac{1}{4}a^2\text{sin}2\theta+C$
  ### $\frac{x}{a}=\text{sin}\theta, \frac{\sqrt{a^2-x^2}}{a^2}=\text{cos}\theta,\text{sin}(\alpha+\beta)=\text{sin}\alpha\text{cos}\beta+\text{sin}\beta\text{cos}\alpha,\text{sin}2\alpha=2\text{sin}\alpha\text{cos}\beta$
  ### $I=\frac{1}{2}a^2\text{sin}^{-1}\frac{x}{a}+\frac{1}{4}a^2\text{sin}2\theta+C=\frac{1}{2}a^2\text{sin}^{-1}\frac{x}{a}+\frac{1}{4}a^22\text{sin}\theta\text{cos}\theta+C=\frac{1}{2}a^2\text{sin}^{-1}\frac{x}{a}+\frac{x}{2}\sqrt{a^2-x^2}+C$

### 예제-4 부정적분  $I=\int_{}^{}\frac{\sqrt{9-x^2}}{x^2}dx$를 구하여라.
+ ### 상기 방식으로는 접근이 어려움. 삼각함수를 고려하여 계산, 항의 제곱 형태
  ###  $Let \quad x=3\text{sin}\theta, dx=3\text{cos}\theta d \theta \quad I=\int_{}^{}\frac{\sqrt{9-x^2}}{x^2}dx=\int_{}^{}\frac{\sqrt{9-9\text{sin}^2\theta}}{3^2\text{sin}^2\theta}3\text{cos}\theta d\theta=\int_{}^{}\frac{\sqrt{9\text{cos}^2\theta}}{3^2\text{sin}^2\theta}3\text{cos}\theta d\theta=\int_{}^{}\frac{\text{cos}^2\theta}{\text{sin}^2\theta}d \theta$
  ###  $I=\int_{}^{}\frac{\text{cos}^2\theta}{\text{sin}^2\theta}d \theta=\int_{}^{}\text{cot}^2\theta d \theta=\int_{}^{}(\text{csc}^2\theta-1)d \theta=-\text{cot}\theta-\theta +C$
  <img src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/7c476384-d7cd-4b10-b0cc-ce20ad13c69d" width=700 />

  ### $I=-\text{cot}\theta-\theta +C=-\frac{\sqrt{9-x^2}}{x}-\text{sin}^{-1}\frac{x}{3}+C$

### 예제-5 부정적분  $I=\int_{}^{}\frac{1}{\sqrt{4+x^2}}dxx$를 구하여라.
+ ### 상기 방식으로는 접근이 어려움. 삼각함수를 고려하여 계산, 항의 제곱 형태
  ###  $Let \quad x=2\text{tan}\theta, dx=2\text{sec}^2\theta d \theta$
  ### $I=\int_{}^{}\frac{2\text{sec}^2\theta}{\sqrt{4+4\text{tan}^2\theta}}d\theta=\int_{}^{}\frac{2\text{sec}^2\theta}{2\text{sec}\theta}d\theta=\int_{}^{}\text{sec}\theta d\theta, \quad(1+\text{tan}^2\theta=\text{sec}^2\theta)$
  ### $\int_{}^{}\text{sec}\theta d\theta=\text{ln}\left| \text{tan}\theta+\text{sec}\theta \right|+C$  [적분 공식 ](https://github.com/DooHub/Electromagnetic_Math/blob/main/Chapt15%EC%A0%81%EB%B6%84%EA%B3%B5%EC%8B%9D.md#13-int_textsecxdxlnleft-textsecxtexttanx-rightc)
  <img src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/9db81dac-e7fb-4fff-b5f7-31622a37ea74" width=700 />

  ### $I=\int_{}^{}\text{sec}\theta d\theta=\text{ln}\left| \text{tan}\theta+\text{sec}\theta \right|+C'=\text{ln}\left| \frac{\sqrt{4+x^2}}{2}+\frac{x}{2} \right|+C'=\text{ln}\left| \sqrt{4+x^2}+x \right|-\text{ln}2+C'\quad (\text{ln}\frac{a}{b}=\text{ln}a-\text{ln}b, C=-\text{ln}2+C')$
  ### x에 상관없이 $\sqrt{4+x^2}>x,sqrt{4+x^2}+x>0 \therefore I=\text{ln}(\sqrt{4+x^2}+x)+C$

### 응용예제
### 공기 중에 점전하 Q로 부터 $\vec{r}$만큼 떨어진 곳에서의 전기장의 세기는 다음과 같다. 
### $\vec{E}=\frac{Q}{4\pi\varepsilon_{0}r^2}\hat{a_{r}}$
### 이로부터 z축에 무한히 긴 필라멘트가 있고, 이 필라멘트의 단위 길이당 전하가 $\rho_{L}\left[ C/m \right]$로 일정할 때 점 $P(\rho,\phi,0)$에서의 전기장의 세기를 구하여라.
<img src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/444779e1-5c6b-44ee-a3c8-a3ae314a7e72" width=700 />

### z=0인 경우 x와 Y평면에 P가 존재하고 Z축에서 X와Y평면으로 향하는 Vector의 크기는 r이 된다 $\hat{a}_{r}=\frac{\vec{r}}{\left| \vec{r} \right|} =\frac{\vec{r}}{r}$
<img src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/30958533-4fb0-486a-8f18-0fb783ed514f" width=1000 />

### $\frac{dQ}{dz}=\rho_{L}\left[ C/m \right],\quad dQ=\rho_{L}dz \quad \vec{E}=\int_{}^{}d\vec{E},\quad d\vec{E}= \frac{dQ}{4\pi\varepsilon_{o}r^2}\hat{a_{r}}=\frac{\rho_{L}}{4\pi\varepsilon_{o}r^3}dz\vec{r}$
<img src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/1de1a5cd-6725-4155-94a8-f03ce0653604" width=1000 />

### $d\overrightarrow{E}=\frac{\rho_{L}}{4\pi\varepsilon_{o}r^3}dz\vec{r}=\frac{\rho_{L}}{4\pi \varepsilon_{o}\left( \rho^2+z^2 \right)^{\frac{3}{2}}}\left( \rho \hat{a_{\rho}}- z\hat{a_{z}}\right)dz$
### x와 Y평면 위에 있는 임의 점 P에 영향을 주는 Z축 위의 전하는 Z가 0일 때를 제외 하고 서로 대칑이 때문에 점P에 관점에서는 서로 상쇄 된다. 즉 $\hat{a_{\rho}}$만 남고 $\hat{a_{z}}$는 z의 +,- 위치의 값에 의해 상쇄 됨 $\overrightarrow{E}= E_{\rho} \hat{a_{\rho}}- E_{z}\hat{a_{z}} \quad\longrightarrow  \overrightarrow{E}= E_{\rho} \hat{a_{\rho}}$
### $d\overrightarrow{E}=\frac{\rho_{L}}{4\pi\varepsilon_{o}\left( \rho^2+z^2 \right)^{\frac{3}{2}}}\left( \rho \hat{a_{\rho}}- z\hat{a_{z}}\right)dz\longrightarrow dE_{\rho}=\frac{\rho_{L}\rho}{4\pi\varepsilon_{o}(\rho^2+z^2)^\frac{3}{2}}dz$
<img src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/bf6a8364-bcec-4297-9e70-e8361e1ee18f" width=1000 />

### $\int_{}^{}dE_{\rho}=\int_{}^{}\frac{\rho_{L}\rho}{4\pi\epsilon_{o}(\rho^2+z^2)^\frac{3}{2}}dz=\frac{\rho_{L}\rho}{4\pi\epsilon_{o}}\int_{}^{}\frac{1}{(\rho^2+z^2)^{\frac{3}{2}}}dz$
<img src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/2132e38b-b01e-49b8-846a-c6bcea8b31ff" width=1000 />


### $\int_{-\infty}^{\infty}\frac{1}{(\rho^2+z^2)^{\frac{3}{2}}}dz, \quad Let \quad z=\rho\text{tan}\theta, \\; dz=\rho\text{sec}^2\theta d \theta  \\; \to \\;    \int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\frac{\rho\text{sec}^2\theta}{(\rho^2+\rho^2\text{tan}^2\theta)^{\frac{3}{2}}}d\theta$
### $\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\frac{\rho\text{sec}^2\theta}{(\rho^2+\rho^2\text{tan}^2\theta)^{\frac{3}{2}}}d\theta=\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\frac{\rho\text{sec}^2\theta}{\rho^3\text{sec}^3\theta}d\theta=\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\frac{1}{\rho^2\text{sec}\theta}d\theta=\frac{1}{\rho^2}\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\text{cos}\theta d\theta, \\;(1+\text{tan}^2\theta=\text{sec}^2\theta)$
### $\frac{1}{\rho^2}\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\text{cos}\theta d\theta=\frac{2}{\rho^2}\int_{0}^{\frac{\pi}{2}}\text{cos}\theta d\theta=\frac{2}{\rho^2}\\;\text{sin}\theta |_{0}^{\frac{\pi}{2}}=\frac{2}{\rho^2}$ cos우함수(Y축 기준 좌우 대칭),sin기함수 성질 이용
### $E_{\rho}=\frac{\rho_{L}\rho}{4\pi\epsilon_{o}}\int_{-\frac{\pi}{2}}^{\frac{\pi}{2}}\frac{1}{\rho^2+z^2}dz=\frac{\rho_{L}\rho}{4\pi\epsilon_{o}}\frac{2}{\rho^2}=\frac{\rho_{L}}{2\pi\epsilon_{o}\rho}$
### 전기장의 세기는 벡터의 값을 가진다. (전기자의 크기와 구분해서 사용)
### $\vec{E}=\frac{\rho_{L}}{2\pi\epsilon_{o}\rho}\hat{a}_{\rho}$
