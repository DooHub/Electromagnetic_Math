## 1. 피적분함수가 무리함수를 포함하는 경우  
###   무리함수를 적분하는 기본적인 방법은 제곱근 기호를 없애는 것이다.
<img src= "https://github.com/DooHub/Electromagnetic_Math/assets/99073912/e4301a91-42a3-482c-9865-d742bfef8443" width=600 />


### 예제-1 부정적분 $I=\int_{}^{}\frac{1}{2x+\sqrt{x}}dx$를 구하여라.
### $Let \quad u=\sqrt{x}=x^{\frac{1}{2}},du=\frac{1}{2}x^{-\frac{1}{2}}dx=\frac{1}{2\sqrt{x}}dx,2udu=dx$
### $I=\int_{}^{}\frac{2u}{2u^2-u}du=\int_{}^{}\frac{2}{2u-1}du=ln\left| 2u \right|+C=ln\left| 2\sqrt{x} \right|+C,\ (\int_{}^{}\frac{1}{ax+b}dx=\frac{1}{a}ln\left| ax+b \right|+C)$
