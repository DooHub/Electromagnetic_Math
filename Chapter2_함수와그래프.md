# 함수에 대한 소개
  - 함수 : 특히 집합 X의 각 원소 x에 집합 Y의 원소 y가 **하나씩 대응될 때** 이 대응을 집합 X에서 집합 Y로의 함수라고 한다.
           만약 특정 x가 대응 되는 y가 두 개 이상이면 함수가 아니다.


### 문제 1
 - 함수 $f(x)=x^{2}$ 에 대하여, $x=5$ 일 때 $\frac{f(x+h)-f(h)}{h}$의 값을 구하라

    $\frac{f(x+h)-f(x)}{h}=\frac{(x+h)^{2}-(x)^{2}}{h} = 2x+h$  
    $\frac{f(5+h)-f(5)}{h}=2\times 5+h =10+h$  
    향후 미분 할 때, 도함수를 구하는 것에 해당함

# 평행이동
 - 함수가 x축 + 방향으로 a만큼 이동하는 한 경우 $x\rightarrow x-a$
 - 함수가 x축 - 방향으로 a만큼 이동하는 한 경우 $x\rightarrow x+a$
 - $y=f(x)$을 x축 + 방향으로 1만큼 이동하면 $y=f(x+1)$함수를 그리면 된다.

## 파동(wave)의 전파(propagation)
### 문제 2 
  - $V_{f}(z,t)=V_{o}\cos(\omega t-\beta z)$는 시간이 지날수록 어느방향으로 진행 하는가?  
  $t=0,   V_{f}(z,0)=V_{o}\cos(0-\beta z) = V_{o}\cos(-\beta z+0)$  
  $t=1,   V_{f}(z,1)=V_{o}\cos(\omega-\beta z) =V_{o}\cos(-\beta (z-\frac{\omega}{\beta})$  
  $t=2,   V_{f}(z,2)=V_{o}\cos(2\omega-\beta z) =V_{o}\cos(-\beta (z-\frac{2\omega}{\beta})$  
  $\omega$와 $\beta$ 모두 상수 이기 때문에 $z-\frac{\omega}{\beta}$는 변수 z에 대한 함수로 볼 수 있고,  
  시간이 변화함(t)에 따라 z의 +방향으로 $\frac{\omega t}{\beta}$ 이동한다고 볼 수 있다. 
