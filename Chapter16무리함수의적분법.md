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
+ ### 상기 방식으로는 접근이 어려움. 삼각함수를 고려하여 계산
  ### $Let \quad x=a\text{sin}\theta,dx=a\text{cos}\theta d \theta, \quad I=\int_{}^{}\sqrt{a^2-a^2\text{sin}^2\theta}a\text{cos}\theta d \theta =\int_{}^{}\sqrt{a^2\text{cos}^2\theta}a\text{cos}\theta d \theta=\int_{}^{}a^2\text{cos}^2\theta d \theta=a^2\int_{}^{}\text{cos}^2\theta d \theta$
  ### 제곱형태의 삼각함수를 제곱이 아닌 형태로 변경 $\text{cos}(\alpha+\beta)=\text{cos}\alpha\text{cos}\beta-\text{sin}\alpha\text{sin}\beta \ ,\text{sin}^2\alpha=1-\text{cos}^2\alpha$
  ### $I=a^2\int_{}^{}\text{cos}^2\theta d \theta=a^2\int_{}^{}\frac{1+\text{cos}2\theta}{2}d \theta=\frac{a^2}{2}\left[ \theta +\frac{1}{2}\text{sin}2\theta \right]+C=\frac{1}{2}a^2\text{sin}^{-1}\frac{x}{a}+\frac{1}{4}a^2\text{sin}2\theta+C$
  ### $\frac{x}{a}=\text{sin}\theta, \frac{\sqrt{a^2-x^2}}{a^2}=\text{cos}\theta,\text{sin}(\alpha+\beta)=\text{sin}\alpha\text{cos}\beta+\text{sin}\beta\text{cos}\alpha,\text{sin}2\alpha=2\text{sin}\alpha\text{cos}\beta$
  ### $I=\frac{1}{2}a^2\text{sin}^{-1}\frac{x}{a}+\frac{1}{4}a^2\text{sin}2\theta+C=\frac{1}{2}a^2\text{sin}^{-1}\frac{x}{a}+\frac{1}{4}a^22\text{sin}\theta\text{cos}\theta+C=\frac{1}{2}a^2\text{sin}^{-1}\frac{x}{a}+\frac{x}{2}\sqrt{a^2-x^2}+C$

### 예제-4 부정적분  $I=\int_{}^{}\frac{\sqrt{9-x^2}}{x^2}dx$를 구하여라.
+ ### 상기 방식으로는 접근이 어려움. 삼각함수를 고려하여 계산
  ###  $Let \quad x=3\text{sin}\theta, dx=3\text{cos}\theta d \theta \quad I=\int_{}^{}\frac{\sqrt{9-x^2}}{x^2}dx=\int_{}^{}\frac{\sqrt{9-9\text{sin}^2\theta}}{3^2\text{sin}^2\theta}3\text{cos}\theta d\theta=\int_{}^{}\frac{\sqrt{9\text{cos}^2\theta}}{3^2\text{sin}^2\theta}3\text{cos}\theta d\theta=\int_{}^{}\frac{\text{cos}^2\theta}{\text{sin}^2\theta}d \theta$
  ###  $I=\int_{}^{}\frac{\text{cos}^2\theta}{\text{sin}^2\theta}d \theta=\int_{}^{}\text{cot}^2\theta d \theta=\int_{}^{}(\text{csc}^2\theta-1)d \theta=-\text{cot}\theta-\theta +C$
  <img src="16_5](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/7c476384-d7cd-4b10-b0cc-ce20ad13c69d" width=300 />
