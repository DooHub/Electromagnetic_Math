# 지수함수
## 지수함의 정의  
 ### 양의 상수 a와 임의의 실수 x에 대하여 $f(x) =a^{x}$ a를 밑으로 하는 지수 함수  
## 지수함수의 성질  
![수학-공식-지수함수-01](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/5fe50e04-3081-460f-97d2-e63cacde480a)
  + 정의역은 실수 전체의 집합이고, 치역은 양의 실수 전체의 집합니다.
  + 그래프는 a에 관계없이 (0,1)을 지난다.
  + 그래프는 x축을 점근선으로 한다.
  + 0<a<1일 때 감소하고, a>1일 때 증가함수 이다.
# 로그함수  
## 로그함수의 정의  
 ### 1이 아닌 모든 양수 a에 대한 $y=a^{x}$의 역함수 $y=log_{a}x$ a를 밑으로 하는 로그 함수
## 로그함수의 성질  
![로그함수vs지수함수](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/98177a0a-3f1e-43e3-8ae2-cf35e4227197)
 + 정의역은 양의 실수 전체의 집합이고, 치역은 실수 전체의 집합이다.
 + 그래프는 a의 값에 상괎없이 (1,0)을 지닌다.
 + 그래프는 y축을 점근선으로 한다.
 + 0<a<1일 때 감소하고, a>1일 때 증가함수 이다.

## 문제  
### Laplace방정식 $\frac{1}{\rho }\frac{\partial }{\partial\rho}(\rho\frac{\partial V}{\partial \rho})=0$을 풀면 $V=Aln\rho+B$ 꼴의 해를 구할 수 있다.  
### 여기에 아래 조건을 적용했을 때의 해들 구하고, a< $\rho$ <b인 구간에서의 그래프를 그려라.   
 + 조건 : $\rho =a$ 에서 $V=V_{o}$, $\rho =b$ 에서  V=0  
   조건을 이용해서 unknown A와 B를 구한다.  
   $\rho=a --> V_{o}=Alna+B,   \therefore B=V_{o}-Alna$  
   $V=Aln\rho+V_{o}-Alna=Aln\frac{\rho}{a}+V_{o}$  
   $\rho=b --> 0=Aln\frac{b}{a}+V_{o}, Aln\frac{b}{a}=-V_{o},\therefore A=\frac{-V_{0}}{ln\frac{b}{a}}$  
   조건을 통해 구한 A와 B를 식에 대입   
   $V=\frac{-V_{0}}{ln\frac{b}{a}}ln\frac{\rho}{a}+V_{o} = V_{o}(1-\frac{ln\frac{\rho}{a}}{ln\frac{b}{a}})$  
   $V_{o}(1-\frac{ln\frac{\rho}{a}}{ln\frac{b}{a}})=V_{o}(\frac{ln\frac{b}{a}-ln\frac{\rho}{a}}{ln\frac{b}{a}})$  
   $V_{o}(\frac{ln\frac{b}{a}-ln\frac{\rho}{a}}{ln\frac{b}{a}})=V_{o}\frac{ln\frac{b}{\rho}}{ln\frac{b}{a}}$  
   $V=V_{o}\frac{ln\frac{b}{\rho}}{ln\frac{b}{a}}$

   ![원통](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/d02fdf7c-e4fe-4d48-8019-d3d1aabc7b35)   
   a와 b 사이의 전화

   ![IMG_2535](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/8489b1bb-66a7-4a0e-9bba-0a9e5aa21ad4)
   
   

