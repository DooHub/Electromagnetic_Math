# 각과 각의 크기
 + 기준선으로부터 반시계방향을 양의 각이라고 하고, 시계방향의 각을 음의 각이라 한다.
 + 사이각은 일반각의 차로 구할 수 있다. 사이각은 항상 양수 이다.
 + 한 바퀴의 각은 360도 로 정의 한다.
 + 반지름이 r일 때 호의 길이가 r이 되는 각을 1 rad으로 정의 한다(호도법). $2\pi rad=360^{\circ}$

# 삼각함수
![tri](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/5f8af861-c68b-430c-b0fc-e87b2dfd28cb)

## x,y는 길이가 아닌 좌표 값 - 위치에 따라 음과 양의 값을 가진다.

# 삼각함수의 기본 성질
## 1) 역수관계 및 상제관계
  ### $csc\theta=\frac{1}{sin\theta}, sec\theta=\frac{1}{cos\theta}, tan\theta=\frac{sin\theta}{cos\theta},cot\theta=\frac{cos\theta}{sin\theta}$
## 2) 제곱 관계
  ### $sin^{2}\theta + cos^{2}\theta = 1$
  ### $1+tan^{2}\theta=sec^{2}\theta, --> 1+(\frac{sin\theta}{cos\theta})^{2}=\frac{cos^{2}\theta+sin^{2}\theta}{cos^{2}\theta}=\frac{1}{cos^{2}\theta}=sec^{2}\theta$
  ### $1+cot^{2}\theta=csc^{2}\theta, -->1+(\frac{cos\theta}{sin\theta})^{2}=\frac{1}{sin^{2}\theta}=csc^{2}\theta$
## 3) 주기 공식    
  ### 임의의 정수 k에 대하여 $sin(2k\pi+\theta)=sin\theta, cos(2k\pi+\theta)=cos\theta, tan(k\pi+\theta)=tan\theta$
## 4) 각 $\frac{n\pi}{2} \pm \theta$ 의 삼각함수
  + $sin(-\theta)= -sin\theta$
  + $cos(-\theta)=cos\theta$
  + $tan(-\theta)=-tan\theta$
  + $sin(\pi -\theta)=sin\theta$
  + $cos(\pi -\theta)=-cos\theta$
  + $tan(\pi -\theta)=-tan\theta$
  + $sin(\frac{\pi}{2}-\theta)=cos(\theta)
  + $cos(\frac{\pi}{2}-\theta)=sin(\theta)
  + $tan(\frac{\pi}{2}-\theta)=cot(\theta)

# 삼각함수의 덧셈 정리
## $cos(\alpha \pm \beta)=cos\alpha cos\beta \mp sin\alpha sin\beta$
#### 증명1 오일러 공식  $e^{j\theta }=cos\theta+jsin\theta$  
$e^{j(\alpha +\beta)} =e^{j\alpha }e^{j\beta }=(cos\alpha+jsin\alpha)(cos\beta+jsin\beta)=(cos\alpha cos\beta -sin\alpha cos\beta)+j(cos\alpha sin\beta +sin\alpha cos\beta)$--식1  
$e^{j(\alpha +\beta)} =cos(\alpha +\beta)+jsin(\alpha +\beta)$ --식2  
식1과 식2는 같다 =실수부와 허수부가 각각 같다  
$\therefore cos(\alpha +\beta)+jsin(\alpha +\beta)=(cos\alpha cos\beta -sin\alpha cos\beta)+j(cos\alpha sin\beta +sin\alpha cos\beta)$  
#### 증명2 Vector 개념 이용
<img width="834" alt="vector" src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/f41ba048-1946-4029-972b-febb72bd8af4">

## $sin(\alpha \pm \beta) = sin\alpha cos\beta \pm sin\beta cos\alpha$
## $tan(\alpha \pm \beta) = \frac{tan\alpha \pm tan\beta}{1 \mp tan\alpha tan\beta}$

## 문제  
### $sin\alpha =\frac{3}{5}, cos\beta=\frac{5}{13}$ 일 때 $tan(\alpha +\beta)$ 을 구하라
