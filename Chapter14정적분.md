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
### 2) $\sum\limits_{k=1}^nk^2=\frac{n(n+1)(2n+1)}{6}$ 증명 하라
### $(n+1)^3-n^3=3n^2+3n+1$ 을 이용하여 n에 $n=1,2, \cdots,n$ 넣은 후에 각 항을 모두 더한다.
<img src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/fb6dc3d3-1459-4579-922d-932104601fc7" width=300 />

### $(n+1)^3-1^3=3(1^2+2^2+\cdots+n^2)+3(1+2\cdots+n)+n\longrightarrow$ 1)
### $1+2+\cdots+n=\frac{n(n+1)}{2},\ Let: \  1^2+2^2+\cdots+n^2=S_n$
### 식1)을 다음과 같이 정리 $n^3+3n^2+3n+1^3-1^3=3S_n+3\frac{n(n+1)}{2}+n$
### $2n^3+6n^2+6n=6S_n+3n^2+5n$
### $2n^3+3n^2+n=n(2n^2+3n+1)=n(n+1)(2n+1)=6S_n \ \therefore \ S_n=\frac{n(n+1)(2n+1)}{6}$

### 3) $\sum\limits_{k=1}^nk^3=[\frac{n(n+1)(2n+1)}{6}]^2$

# 2. 구분구적법
### 함수 $f(x)=x^2$의 그래프와 x축, 그리고 직선 x=0과 x=1로 둘러싸인 도형의 넓이 S를 구하라. 
### (구분구적법으로) $S_k\to S_n\to S=\underset{n \to \infty }{\text{lim}} S_n$
<img src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/107a6a23-caae-4016-b835-46727f87b2ad" width=800 />

### k번째 직사가격의 넓이는 $S_k=\frac{1}{n}(\frac{k}{n})^2\ $ n조각의 $S_k$합은 $S_n=\sum\limits_{k=1}^n S_k$
