# ICE Breaking - 삼각함수 적용 되는 경우
공간을 진행하는 전자기파는 전기장과 자기장이 함께 존재하고, 전자기파는 에너지를 빛의 속도로 전파(Propagation)한다.  
전자기파가 공간으로 나르는 전력을 평균전력밀도로 나타낸다.

### $< S_{z} >=\frac{1}{T}\int_{T}^{0}E_{x}H_{y}dt=\frac{1}{2}\frac{E_{xo}^{2}}{\left | \eta  \right |}e^{-2az}cos\theta _{\eta }$
+ 상기 적분과정에서 삼각함수의 공식이 이용 된다.

## 1.배각의 공식
 + $sin2\alpha = 2sin\alpha cos\alpha \leftarrow sin(\alpha \pm \beta)=sin\alpha cos\beta \pm sin\beta cos\alpha$
 + $cos2\alpha =2cos^{2}\alpha -1 =1-2sin^{2}\alpha \leftarrow cos(\alpha \pm \beta)=cos\alpha cos\beta \mp sin\alpha cos\beta ( sin^{2}\theta + cos^{2}\theta=1, cos^{2}\theta=1- sin^{2}\theta)$
 + $tan2\alpha = \frac{2tan\alpha}{1-tan^{2}\alpha} \leftarrow tan(\alpha \pm \beta)=\frac{tan\alpha \pm tan\beta}{1 \mp tan\alpha tan\beta}$

## 2.반각의 공식
 + $cos^{2}\alpha =\frac{1}{2}(1+cos2\alpha)$
 + $sin^{2}\alpha=\frac{1}{2}(1-cos2\alpha)$
 + $tan^{2}=\frac{1-cos2\alpha}{1+cos2\alpha}$ 위 두 공식 적용
### 문제1
 + $cos^{2}22.5^{\circ}$ 계산기 없이 풀어라  
   $cos^{2}\alpha =\frac{1}{2}(1+cos2\alpha) \rightarrow=\frac{1}{2}(1+cos45^{\circ})=\frac{2+\sqrt{2}}{4})$

## 3.곱을 합 또는 차로 고치기
 + $cos(\alpha+\beta)+cos(\alpha-\beta)=2cos\alpha cos\beta$
 + $sin(\alpha+\beta)+sin(\alpha-\beta)=2sin\alpha cos \beta$
### 문제2
 + $cos75^{\circ}cos15^{\circ}$ 계산기 없이 풀어라  
   $cos(75^{\circ} +15^{\circ}),cos(75^{\circ} -15^{\circ})$을 이용하여 계산 한다.  
   $cos(75^{\circ} +15^{\circ})=cos75^{\circ}cos15^{\circ} -sin75^{\circ}sin15^{\circ} ----1)$  
   $cos(75^{\circ} -15^{\circ})=cos75^{\circ}cos15^{\circ} +sin75^{\circ}sin15^{\circ} ----2)$  
   1)과 2)를 더하면 $2cos75^{\circ}cos15^{\circ}=cos(90^{\circ})+cos(60^{\circ}) =\frac{1}{4}$
### 문제3
  + $sin75^{\circ}+sin15^{\circ}$계산기 없이 풀어라  
    $75^{\circ}=45^{\circ}+30^{\circ},15^{\circ}=45^{\circ}-30^{\circ}$아는 각으로 변경, 배각 공식에 적용  
    $sin(\alpha+\beta)=sin(\alpha)cos(\beta)+sin(\beta)cos(\alpha)\rightarrow 1)$  
    $sin(\alpha-\beta)=sin(\alpha)cos(\beta)-sin(\beta)cos(\alpha)\rightarrow 2)$
    1)과 2) 더하고 $\alpha=40^{\circ},\beta=15^{\circ}$ 설정  
    $sin75^{\circ}+sin15^{\circ}=2sin(45^{\circ})cos(30^{\circ})=2\frac{\sqrt{2}}{2}\frac{\sqrt{3}}{2}=\frac{\sqrt{6}}{2}$
### 응용문제  
전기장 $E_{x}$와 자기장 $H_{y}$가 다음과 같이 주어졌다.  
$E_{x}=E_{x0}e^{-\alpha z}cos(\omega t-\beta z), \quad H_{y}=\frac{E_{xo}}{\left | \eta  \right |}e^{-\alpha z}cos(\omega t-\beta z-\theta_{\eta} )$  
![EH_z](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/211e79e6-6d93-421f-bf99-019a4271f51c)  
이때 +z방향으로 전달되는 평균전력밀도 $< S_{z} >=\frac{1}{T}\int_{0}^{T}E_{x}H_{y}dt$라고 할 때, $< S_{z} >$을 풀이한 결과가 $\frac{1}{2}\frac{E_{xo}^{2}}{|\eta |}e^{-2\alpha z}cos\theta _{\eta }$와 같이 됨을 보여라.  
+ $< S_{z} >=\frac{1}{T}\int_{0}^{T}E_{x0}e^{-\alpha z}cos(\omega t-\beta z)\frac{E_{xo}}{\left | \eta  \right |}e^{-\alpha z}cos(\omega t-\beta z-\theta _{\eta})dt$  
  dt에 대해 적분하기 때문에 변수 t를 제외하고는 상수로 취급하여 적분 기호 앞으로 추출 가능  
- $\frac{1}{T}\frac{E_{xo}^{2}}{\left | \eta  \right |}e^{-2\alpha z}\int_{0}^{T}cos(\omega t-\beta z)cos(\omega t-\beta z-\theta _{\eta})dt$  ---1)
- $cos(\alpha \pm \beta)=cos\alpha cos\beta \mp sin \alpha sin \beta, \quad \frac{1}{2}[ cos(\alpha + \beta)+cos(\alpha - \beta) ] =cos\alpha cos\beta$  위에 적용
- $\omega t-\beta z = \alpha, \omega t-\beta z-\theta _{\eta}=\beta$라고 하면
- $\int_{0}^{T}cos(\omega t-\beta z)cos(\omega t-\beta z-\theta _{\eta})dt=$ $\int _{0}^{T}\frac{1}{2}[cos(2\omega t-2\beta z-\theta _{\eta})+cos(\theta _{\eta})]dt$ 
- $\int _{0}^{T}\frac{1}{2}[cos(2\omega t-2\beta z-\theta _{\eta})+cos(\theta _{\eta})]dt = \frac{1}{2}\int _{0}^{T}cos(2\omega t-2\beta z-\theta _{\eta})dt + \frac{1}{2}\int _{0}^{T}cos(\theta _{\eta})]dt$
- $\frac{1}{2}\int _{0}^{T}cos(2\omega t-2\beta z-\theta _{\eta})dt$는 cos(\omega t)가 대비 주기가 $\frac{1}{2}$ 줄어들어 T 동안 두번 반복 된다. 하지만 결국 주기를 적분하기 때문에 값은 0 이 된다.  
![image](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/357d737e-4afe-4933-b5df-913da525a98f)
- $\frac{1}{2}\int _{0}^{T}cos(\theta _{\eta})]dt =\frac{T}{2}cos(\theta _{\eta})]dt$가 된다.
- $\therefore \int_{0}^{T}cos(\omega t-\beta z)cos(\omega t-\beta z-\theta _{\eta})dt =\frac{T}{2}cos(\theta _{\eta})]dt$ 가 되고 이를 1)에 대입 하면, $\frac{1}{2}\frac{E _{xo}^{2}}{|\eta |}e^{-2\alpha z}cos\theta _{\eta }$ 구할 수 있다




    
   

