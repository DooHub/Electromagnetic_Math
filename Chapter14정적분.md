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

### k번째 직사가격의 넓이는 $S_k=\frac{1}{n}(\frac{k}{n})^2 \quad$ n조각의 $S_k$합은 $S_n=\sum\limits_{k=1}^n S_k$
### $S_n=\sum\limits_{k=1}^n S_k=\sum\limits_{k=1}^n \frac{1}{n}(\frac{k}{n})^2=\frac{1}{n^3}\sum\limits_{k=1}^n k^2=\frac{1}{n^3}\times \frac{n(n+1)(2n+1)}{6}=\frac{(n+1)(2n+1)}{6n^2}$
### $S=\underset{n \to \infty }{\text{lim}}S_n=\underset{n \to \infty }{\text{lim}}\frac{(n+1)(2n+1)}{6n^2}=\underset{n \to \infty }{\text{lim}}\frac{(1+\frac{1}{n})(2+\frac{1}{n})}{6}=\frac{1}{3}$


## 예제-1
### 밑변의 길이가 a, 높이가 h인 삼각형의 넓이 S를 구분구적법을 이용하여 구하라.
![triangle](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/41f807b9-0de1-48bc-aabb-0fa1c04fbd5e)

### $S_k=\frac{a}{n}k\frac{h}{n}=\frac{ah}{n^2}k, \quad S_n=\sum\limits_{k=1}^n S_k=\sum\limits_{k=1}^n \frac{ah}{n^2}k=\frac{ah}{n^2}\sum\limits_{k=1}^n k=\frac{ah}{n^2}\frac{n(n+1)}{2}=\frac{ah(n+1)}{2n}$
### $S=\underset{n \to \infty }{\text{lim}}S_n=\underset{n \to \infty }{\text{lim}}\frac{ah(n+1)}{2n}=\frac{ah}{2}\underset{n \to \infty }{\text{lim}}\frac{1+\frac{1}{n}}{1}=\frac{1}{2}ah$

## 예제-2
### 반지름의 길이가 r인 원의 넓이 S를 구분구적법을 이용하여 구하라.
![circle](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/17465828-77b5-4f09-9708-80c35a9d06b3)


### n개의 삼각형이 원 안에 있을 경우, 원의 넓이는 삼각형의 넓이 n개 있는 것이랑 동일 함.
### $S_k=\frac{1}{2}(2a)h=ah=r\text{sin}\frac{\theta}{2}\times r\text{cos}\frac{\theta}{2}=r^2\text{sin}\frac{\theta}{2}\text{cos}\frac{\theta}{2}=\frac{1}{2}r^2\text{sin}\theta, \quad[\text{sin}(\alpha+\beta)=\text{sin}\alpha\text{cos}\beta+\text{sin}\beta\text{cos}\alpha]$
### $S_n=\sum\limits_{k=1}^n S_k=\sum\limits_{k=1}^n \frac{1}{2}r^2\text{sin}\theta=\frac{1}{2}nr^2\text{sin}\theta=\frac{1}{2}nr^2\text{sin}\frac{2\pi}{n}$
### $S=\underset{n \to \infty }{\text{lim}}S_n=\underset{n \to \infty }{\text{lim}}\frac{1}{2}nr^2\text{sin}\frac{2\pi}{n}=\underset{n \to \infty }{\text{lim}}\frac{\text{sin}\frac{2\pi}{n}}{\frac{2\pi}{n}}\pi r^2=\pi r^2\underset{n \to \infty }{\text{lim}}\frac{\text{sin}\frac{2\pi}{n}}{\frac{2\pi}{n}}$
### $Let, \ x=\frac{2\pi}{n}, n \to \infty, \ x \to 0, \quad S=\pi r^2\underset{x \to 0 }{\text{lim}}\frac{\text{sin}x}{x}=\pi r^2, \quad (\underset{x \to 0 }{\text{lim}}\frac{\text{sin}x}{x}=1)$ [삼각함수도함수](https://github.com/DooHub/Electromagnetic_Math/blob/main/Chapter11%EC%82%BC%EA%B0%81%ED%95%A8%EC%88%98%EC%9D%98%EB%8F%84%ED%95%A8%EC%88%98.md)

# 3. 정적분
### 함수가 일 때, 곡선 y=f(x)와 x축 및 x=a, x=b(b>a)로 둘러싸인 영역의 넓이 S를 구분구적법으로 구해라.
![Integral](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/233d304f-6f00-4da5-b7dd-c4d2980764aa)

### $\Delta x=\frac{b-a}{n}, \ x_k=a+\Delta x k\ \longrightarrow \ S_k=\Delta xf(x_k), \ S_n=\sum\limits_{k=1}^n S_k=\sum\limits_{k=1}^n \Delta xf(x_k)$
### $S=\underset{n \to \infty }{\text{lim}}S_n=\underset{n \to \infty }{\text{lim}}\sum\limits_{k=1}^n \Delta xf(x_k)$
________________________________________________________________________________________________________________________
### 상기 구한 결과 $S=\underset{n \to \infty }{\text{lim}}\sum\limits_{k=1}^n \Delta xf(x_k)$를 다음과 같이 정의 하고 이를 정적분이라고 한다.
+ ### $\int_{a}^{b}f(x)dx=\underset{n \to \infty }{\text{lim}}\sum\limits_{k=1}^n \Delta xf(x_k), \ x_k=a+k\Delta x, \ \Delta x=\frac{b-a}{n}$

## 예제-3
### $\int_{0}^{2}x^3dx$의 값을 정적분의 정의에 의하여 구하라
+ ### $\underset{n \to \infty }{\text{lim}}\sum\limits_{k=1}^n \Delta xf(x_k),\ \Delta x =\frac{b-a}{n},\ x_k=a+\Delta x k$
+ ### $\Delta x=\frac{2}{n}, \ x_k=\frac{2}{n}k, \ \sum\limits_{k=1}^n \Delta xf(x_k)=\sum\limits_{k=1}^n \frac{2}{n}(\frac{2}{n}k)^3=\frac{16}{n^4}\sum\limits_{k=1}^nk^3=\frac{16}{n^4}[\frac{n(n+1)}{2}]^2$
