# 지수
1. 지수의 정의  
 실수 a와 양의 정수 n에 대하여 a를 n번 곱한 것을 a의 n제곱이라고 한다.
  + $a^{m}=N$ --->  &nbsp;&nbsp;a:밑    &nbsp;&nbsp;n: 지수
2. 지수법칙  
  a>0, b>0이고 m,n 이 정수 일 때, 다음과 같은 성질이 성립한다.
  + $a^{\frac{m}{n}}=\sqrt[n]{a^{m}}$
  + $\left ( a^{m} \right )^{n}=a^{mn}=\left ( a^{n} \right )^{m}$
3. 거듭제곱근의 성질  
  a>0, b>0이고, m,n이 1보다 큰 정수 일 때  
-- 전하에 일정 거리의 전계를 구할 때 분모와 분자 부분 거리 정리 할 때 사용
  + $\sqrt[n]{a}\sqrt[n]{b}=\sqrt[n]{ab}$
  + $\frac{{}\sqrt[n]{a}}{\sqrt[n]{b}}=\sqrt[n]{\frac{a}{b}}$
  + $\left ( \sqrt[n]{a} \right )^{m}=\sqrt[n]{a^{m}}$
  + $\sqrt[m]{\sqrt[n]{a}}=\sqrt[mn]{a}=\sqrt[n]{\sqrt[m]{a}}$
  + $\sqrt[np]{a^{mp}}=\sqrt[n]{a^{m}}$

# 로그  
지수는 매우 큰 수나 매우 작은 수를 표현 할수 있지만, 그래프로 표현하기 어렸다.  
로그를 이용하면 위와 같은 문제를 해결 할 수 있다.

1. 로그의 정의  
  $a>0, a\neq1$ 이고 N>0일 때, $a^{m}=N$을 만족하는 m은 오직 하나 존재 한다.
  수학적으로 a는 0보다 작을 수 있으나, **공학에서는 안정화(수렴 또는 계산이 되는)를 고려하여 a가 음수 일 때는 고려 안 함.**
  + $a^{m}=N \Leftarrow \Rightarrow m = log_{a}N $  
   N:진수(argument) &nbsp;&nbsp;m(Exponent):a를 밑으로 하는 N의 로그 &nbsp;&nbsp;The logarithm, base a of N  
   상용 로그 = Common log
2. 로그의 성질  
$a>0, a\neq1, M>0, N>0$ 일 때
  + $log_{a}a=1$
  + $log_{a}1=0$
  + $log_{a}MN=log_{a}M+log_{a}N$
  + $log_{a}\frac{M}{N}=log_{a}M-log_{a}N$
  + $log_{a}M^{n}=nlog_{a}M$&nbsp;$&nbsp;(n은 실수)
3. 밑변환 공식  
$a>0, a\neq1, c>0, c\neq1,b>0$ 일 때
  + $log_{a}b=\frac{log_{c}b}{log_{c}a}$    
    $\textbf{Let :}  A=log_{a}b, a^{A}=b --> log_{c}a^{A}=log_{c}b --> Alog_{c}a=log_{c}b --> A=\frac{log_{c}b}{log_{c}a} $
  + $log_{a}b=\frac{1}{log_{b}a} (b>0, b\neq1)--->  log_{a}b=\frac{log_{b}b}{log_{b}a} , log_{b}b=1$
  + $a^{log_{b}c}=c^{log_{b}a} (b>0, b\neq1, c>0)$  
    $\textbf{Let :}  A=a^{log_{b}c} --> log_{a}A=log_{b}c$ &nbsp;,&nbsp; $\frac{log_{c}A}{log_{c}a}=\frac{log_{c}c}{log_{c}b}=\frac{1}{log_{c}b}$  
    $log_{c}A=\frac{log_{c}a}{log_{c}b} = log_{b}a$ &nbsp;,&nbsp; $A=c^{log_{b}a}$
  + $log_{a^{m}}M^{n}=\frac{n}{m}log_{a}{M}$ (m,n은 실수이고, $m=\neq0$)   
     $\textbf{Let :}  A=log_{a^{m}}M^{n}  --> (a^{m})^{A}=M^{n}$
     $()^{\frac{1}{n}}  ==> (a^{mA})^{\frac{1}{n}}=(M^{n})^{\frac{1}{n}} , a^{\frac{m}{n}A}=M, log_{a}a^{\frac{m}{n}A}=log_{a}M$
     $\frac{m}{n}A =log_{a}M ==> A=\frac{n}{m}log_{a}M$
 ## 문제1  
 $log_{10}2=a, log_{10}3=b$라 할 때 다음 식의 값을  a,b로 나타내어라  
   + $log_{10}\sqrt{30}$   
     $log_{10}30^{\frac{1}{2}}=\frac{1}{2}log_{10}(3\times 2 \times 5)=\frac{1}{2}(log_{10}3+log_{10}2+log_{10}5), log_{10}5=log_{10}\frac{10}{2}=log_{10}10-log{10}2$  
     $\frac{1}{2}(log_{10}3+log_{10}2+ log_{10}10-log_{10}2) =\frac{1}{2}(b+a+1-a)=\frac{1}{2}(b+1) $
   + $log_{10}0.72$  
     $log_{10}\frac{72}{100}=log_{10}(2^{3}x3^{2})-log_{10}10^{2}=3log_{10}2+2log_{10}3-2log_{10}10=3a+2b-2$
   + $log_{9}4$  
     $log_{3^{2}}2^{2}=\frac{2}{2}log_{3}2=\frac{a}{b}$

 ## 문제2  
  반사 계수 구할 때 활용  
  + $e ^{2x}=3$일 때,  $\frac{e^{3x}+e^{-3x}}{e^{x}+e^{-x}}$ 구하라    
  ### $\frac{e^{-3x}(e^{6x}+1)}{e^{-x}(e^{2x}+1)} = \frac{e^{-2x}(e^{6x}+1)}{(e^{2x}+1)}$
  ### $=\frac{e^{-2x}((e^{2x})^{3}+1)}{(e^{2x}+1)}=\frac{1}{3}\times \frac{27+1}{3+1}=\frac{7}{3}$

  # 자연로그 (natural logarithm)   
  1. 무리수 e의 정의 
   ####  $e = \lim_{n\rightarrow \infty }\left ( 1+\frac{1}{n} \right )^{n}$  
   ####  $( 1+\frac{1}{10})^{10} = 2.5937 \cdot \cdot \cdot$  
   ####  $( 1+\frac{1}{1000})^{1000} = 2.7169 \cdot \cdot \cdot$  
   ####  $e = 2.71828182 \cdot \cdot \cdot$  -->무리수
  2. 자연 로그  
   #### $log_{e}x=lnx$
   #### $e^{x}$의 경우 미분과 적분을 해도 결과가 $e^{x}$ 자신이 된다 -->공학에서 많이 사용하는 이유 중 하나
   ####  . $e^{lnx}=x (x>0)$  
   ####  . $lne^{x}=x $
 ## 문제3  
 ### $5lnx+3lny-4lnz$을 간단히 하여라  
 ### --> $lnx^{5} + lny^{4} - lnz^{4} =ln\frac{x^{5}y^{4}}{z^{4}}$
