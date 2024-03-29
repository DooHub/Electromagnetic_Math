# 1. 적분 공식
### 1) $\int_{}^{}x^ndx=\frac{1}{n+1}x^{n+1}+C$ (단, $n\neq =1$)
### 2) $\int_{}^{}\frac{1}{x}dx=ln\left| x \right|+C$
### 3) $\int_{}^{}e^xdx=e^x+C$
### 4) $\int_{}^{}a^xdx=\frac{a^x}{lna}+C$
### 5) $\int_{}^{}\text{cos}xdx=\text{sin}x+C$
### 6) $\int_{}^{}\text{sin}xdx=-\text{cos}x+C$
### 7) $\int_{}^{}\text{sec}^2xdx=\text{tan}x+C$
### 8) $\int_{}^{}\text{csc}^2xdx=-\text{cot}x+C$
### 9) $\int_{}^{}\text{sec}xd\text{tan}xdx=\text{sec}x+C$
### 10) $\int_{}^{}\text{csc}xd\text{cot}xdx=-\text{csc}x+C$
### 11) $\int_{}^{}\text{tan}xdx=-ln\left| \text{cos}x\right|+C$
### 12) $\int_{}^{}\text{cot}xdx=ln\left| \text{sin}x\right|+C$
### 13) $\int_{}^{}\text{sec}xdx=ln\left| \text{sec}x+\text{tan}x \right|+C$
### 14) $\int_{}^{}\text{csc}xdx=ln\left| \text{csc}x-\text{cot}x \right|+C$
### 15) $\int_{}^{}\frac{1}{\sqrt{1-x^2}}dx=\text{sin}^{-1}x+C$
### 16) $\int_{}^{}\frac{1}{1+x^2}dx=\text{tan}^{-1}x+C$

# 2. 활용법
### 1)~8)까지는 외우고 나머지는 유도 과정을 익혀서 모델링 할 때 적용
+ ### 12)의 경우   $\int_{}^{}\text{cot}xdx=ln\left| \text{sin}x\right|+C$
  ### $\int_{}^{}\text{cot}xdx=\int_{}^{}\frac{\text{cos}x}{\text{sin}x}dx, \quad(u=\text{sin}x,du=\text{cos}xdx)$
  ### $\int_{}^{}\frac{1}{u}du=ln\left| u \right|+C,(u=\text{sin}x) \quad \therefore \int_{}^{}\text{cot}xdx=ln\left| \text{sin}x \right|+C$
+ ### 13)의 경우 $\int_{}^{}\text{sec}xdx=ln\left| \text{sec}x+\text{tan}x \right|+C$
  ### $\int_{}^{}\text{sec}xdx=\int_{}^{}\frac{1}{\text{cos}x}dx=\int_{}^{}\frac{\text{cos}x}{\text{cos}^2x}dx=\int_{}^{}\frac{\text{cos}x}{1-\text{sin}^2x}dx, \ (1=\text{sin}^2x+\text{cos}^2x)$
  ### $u=\text{sin}x, du=\text{cos}xdx, \quad \int_{}^{}\frac{\text{cos}x}{1-\text{sin}^2x}dx\longrightarrow \int_{}^{}\frac{1}{1-u^2}du=\int_{}^{}\frac{1}{(1-u)(1+u)}du$
  ### $\frac{1}{(1-u)(1+u)}=\frac{A}{(1-u)}+\frac{B}{(1+u)}, (A=\frac{1}{2},B=\frac{1}{2}), \longrightarrow \int_{}^{}\frac{1}{(1-u)(1+u)}du=\frac{1}{2}\int_{}^{}(\frac{1}{1-u}+\frac{1}{1+u})du$
  ### $\frac{1}{2}\int_{}^{}(\frac{1}{1-u}+\frac{1}{1+u})du=\frac{1}{2}\left[ ln\left| 1+u \right| -ln\left| 1-u \right|\right]+C=\frac{1}{2}ln\left| \frac{1+u}{1-u} \right|+C$
  ### $\frac{1+\text{sin}x}{1-\text{sin}x}=\frac{(1+\text{sin}x)^2}{1-\text{sin}^2x}=\frac{(1+\text{sin}x)^2}{\text{cos}^2x}=\left[  \frac{(1+\text{sin}x)}{\text{cos}x} \right]^2=(\text{sec}x+\text{tan}x)^2$
  ### $\int_{}^{}\text{sec}xdx=\frac{1}{2}ln\left| \frac{1+\text{sin}x}{1-\text{sin}x} \right|+C=\frac{1}{2}ln(\text{sec}x+\text{tan}x)^2+C=ln\left| \text{sec}x+\text{tan}x  \right|+C$
+ ### 15)의 경우 $\int_{}^{}\frac{1}{\sqrt{1-x^2}}dx$
  ### $x=\text{sin}\theta, \ dx=\text{cos}\theta d\theta \quad (\theta=\text{sin}^{-1}x,\text{sin}^{-1}x=\text{arcsin}x)$
  ### $\int_{}^{}\frac{1}{\sqrt{1-x^2}}dx=\int_{}^{}\frac{\text{cos}\theta}{\sqrt{1-\text{sin}^2\theta}}d \theta=\int_{}^{}\frac{\text{cos}\theta}{\text{cos}\theta}d \theta=\int_{}^{}d \theta=\theta+C=\text{sin}^{-1}x+C, \ (1-\text{sin}^2 \theta=\text{cos}^2\theta)$

+ ### 16)의 경우 $\int_{}^{}\frac{1}{1+x^2}dx=\text{tan}^{-1}x+C$
  ### $x=\text{tan}\theta, \ dx=\text{sec}^2\theta d\theta \quad (\theta=\text{tan}^{-1}x,\text{tan}^{-1}x=\text{arctan}x)$
  ### $\int_{}^{}\frac{1}{1+x^2}dx=\int_{}^{}\frac{\text{sec}^2\theta}{1+\text{tan}^2\theta}d \theta=\int_{}^{}d \theta=\theta+C=\text{tan}^-1x,\ (\text{sec}^2\theta=1+\text{tan}^2\theta)$
# 예제
## 예제-1 부정적분 $I=\int_{}^{}\frac{x}{\text{sin}^2x^2}dx$
+ ### $u=x^2, \ du=2xdx \quad I=\int_{}^{}\frac{1}{2}\frac{1}{\text{sin}^2u}du=\frac{1}{2}\int_{}^{}\text{csc}^2udu=-\frac{1}{2}\text{cot}u+C=-\frac{1}{2}\text{cot}x^2+C$
## 예제-2 부정적분 $I=\int_{}^{}\frac{3}{\sqrt{1-4x^2}}dx$
+ ### $\text{Let} \ 2x=\text{sin}\theta, \ (1-\text{cos}^2\theta=\text{sin}^2\theta)$
  ### <img src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/bff33658-74b1-4c53-be15-fbbf6dfe6d51" width=800 />

  ### $2dx=\text{cos}\theta d\theta, \quad I=\int_{}^{}\frac{3}{\sqrt{1-\text{sin}^2\theta}}\frac{1}{2}\text{cos}\theta d\theta=\frac{3}{2}\int_{}^{}\frac{\text{cos}\theta}{\text{cos}\theta}d \theta=\frac{3}{2}\theta+C=\frac{3}{2}\text{sin}^{-1}2x+C$
## 예제-3 부정적분 $I=\int_{}^{}\frac{2}{x^2-4x+8}dx$
+ ### $x^2-4x+8=(x-2)^2+2^2, \ \text{Let} \ x-2=2\text{tan}\theta, \ dx=2\text{sec}^2\theta d\theta$
  ### $I=\int_{}^{}\frac{2}{4\text{tan}^2\theta+4}2\text{sec}^2\theta d\theta=\int_{}^{}\frac{\text{sec}^2\theta}{\text{sec}^2\theta}d \theta=\theta+C=\text{tan}^{-1}\frac{x-2}{2}+C, \ (\text{tan}^2\theta+1=\text{sec}^2\theta)$
  
