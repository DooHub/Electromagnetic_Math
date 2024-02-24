# 1. 수열의 합
### 1) $\sum\limits_{k=1}^nk=\frac{n(n+1)}{2}$ 증명 하라
* ### 방법 1
### $\ 1+2+3+\cdots +(n-1)+n\longrightarrow$    1)
### $\ n+(n-1)+\cdots 3+2+1\longrightarrow$     2)
### 1)과 2)를 더하면 $n(n+1)$이 되고, 이를 반으로 나눈 값이 $\frac{n(n+1)}{2}$가 된다
* ### 방법 2
### $(n+1)^2-n^2=2n+1$ 을 이용하여 n에 $n=1,2, \cdots,n$ 넣은 후에 각 항을 모두 더한다.
<img src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/920e15e5-a4d3-4271-a583-4c26387b3f2d" width=300 />

### $(n+1)^2-1^2=2(1+2+\cdots+n)+n, \quad Let: \ (1+2+\cdots+n)=S_n$
### $(n+1)^2-1^2=2S_n+n\longrightarrow n^2+2n+1^2-1^2-n=n(n+1)=2S_n \ \therefore \frac{n(n+1)}{2}=S_n$
________________________________________________
### 2) $\sum\limits_{k=1}^nk^2=\frac{n(n+1)(2n+1}{6}$ 증명 하라
### $(n+1)^3-n^3=3n^2+3n+1$ 을 이용하여 n에 $n=1,2, \cdots,n$ 넣은 후에 각 항을 모두 더한다.


### $(n+1)^3-1^3=3(1^2+2^2+\cdots+n^2)+3(1+2\cdots+n)+n\longrightarrow$ 1)
### $1+2+\cdots+n=\frac{n(n+1)}{2},\ Let: \  1^2+2^2+\cdots+n^2=S_n$
### 식1)을 다음과 같이 정리 $n^3+3n^2+3n+1^3-1^3=3S_n+3\frac{n(n+1)}{2}+n$
### $2n^3+6n^2+6n=6S_n+3n^2+5n$
### $2n^3+3n^2+n=n(2n^2+3n+1)=n(n+1)(2n+1)=6S_n \ \therefore \ S_n=\frac{n(n+1)(2n+1)}{6}$
