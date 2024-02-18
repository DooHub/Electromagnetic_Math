## 치환적분법
### $I=\int_{}^{}x^3\sqrt{x^4+4}dx$가 $\frac{1}{6}(x^4+4)^{\frac{3}{2}}+C$ 이 됨을 보여라
+ ### Let $u=x^4+4, \ du=4x^3dx, \frac{1}{4}=x^3dx, \ \longrightarrow I=\int_{}^{}\frac{1}{4}\sqrt{u}du =\frac{1}{4}\int_{}^{}u^{\frac{1}{2}}du=\frac{1}{6}u^{\frac{3}{2}}+C = \frac{1}{6}(x^4+4)^{\frac{3}{2}}+C$
### $I=\int_{}^{}2xe^{x^2}dx$구하라
+ ### Let $u=x^2, \ du=2xdx,\ \longrightarrow I=\int_{}^{}e^udu=e^u+C=e^{x^2}+C$

## 부분적분
### $\int_{}^{}f(x)g'(x)dx=f(x)g(x)-\int_{}^{}f'(x)g(x)dx$ 이 됨을 보여라
+ ### $\\{ f(x)g(x) \\}'=f'(x)g(x)+f(x)g'(x) \ \longrightarrow \int_{}^{}\\{f(x)g(x) \\}'dx=\int_{}^{}f'(x)g(x)dx+\int_{}^{}f(x)g'(x)dx$
  ### $f(x)g(x)=\int_{}^{}f'(x)g(x)dx+\int_{}^{}f(x)g'(x)dx$
### $u=f(x),v=g(x), \quad du=u'dx, dv=v'dx \ \longrightarrow  \int_{}^{}uv'dx=uv-\int_{}^{}vdu$ 치환적분 간략화
+ ### $I=\int_{}^{}lnxdx, \ u=lnx, du=\frac{1}{x}dx, v=x, dv=dx, \ \longrightarrow I=uv-\int_{}^{}vdu=xlnx - x +C$
## 예제-1
### $I=\int_{}^{}\frac{(\text{tan}^{-1} x)^2}{1+x^2}dx$ 구하라
+ ### $\text{tan}\theta=x, \ \longrightarrow \ \frac{d}{dx}(\text{tan}\theta)=\frac{d(\text{tan}\theta)}{d\theta}\frac{d\theta}{dx}=\text{sec}^{2}\theta \frac{d\theta}{dx} ,\ \frac{d}{dx}(\text{tan}\theta)=\frac{d}{dx}(x)=1, \ \therefore \text{sec}^{2}\theta \frac{d\theta}{dx}=1$
+ ### $\theta =\text{tan}^{-1}x,\ \longrightarrow \ \frac{d\theta}{dx}=\frac{d}{dx}(\text{tan}^{-1}x)=\frac{1}{\text{sec}^{2}\theta}=\text{cos}^{2}=\frac{1}{x^2+1}, \ d\theta=\frac{1}{x^2+1}dx$
+ ### $I=\int_{}^{}\frac{(\text{tan}^{-1} x)^2}{1+x^2}dx=\int_{}^{}\theta^2d\theta=\frac{1}{3}\theta^3+C=\frac{1}{3}(\text{tan}^{-1}x)^3+C$
<img src="https://github.com/DooHub/Electromagnetic_Math/assets/99073912/b858be27-edb3-4730-b2c5-4c2a2e92dc86" />

## 예제-2
### $I=\int_{}^{}e^{2x}\text{sin}xdx$ 구하라
+ ### $u=e^{2x},dv=\text{sin}{x}dx, \ du=2e^{2x}dx,v=-\text{cos}x$
+ ### $I=-e^{2x}\text{cos}x + \int_{}^{}\text{cos}x2e^{2x}dx$
+ ### $u=2e^{2x},dv=\text{cos}xdx,du=4e^{2x}dx,v=\text{sin}x$
+ ### $\int_{}^{}\text{cos}x2e^{2x}dx=2e^{2x}\text{sin}x-\int_{}^{}\text{sin}x4e^{2x}dx,\quad -4\int_{}^{}e^{2x}\text{sin}xdx=4I$
+ ### $I=-e^{2x}\text{cos}x + \int_{}^{}\text{cos}x2e^{2x}d=-e^{2x}\text{cos}x +2e^{2x}\text{sin}x -4I$
  ### $\ \ =\frac{-1}{5}e^{2x}\text{cos}x +\frac{2}{5}e^{2x}\text{sin}x+C$


## 응용예제
### 전위(electric potential)를 구하는 과정에서 전위 V는 $V=V_{+}+V_{-}$ 로 나타 낼 수 있다.
### $V_{+}=-\frac{\rho_{L}}{2\pi\varepsilon_{0}}\int_{4}^{7}\frac{x-6}{(x-6)^{2}+16}dx$
### $V_{-}=\frac{\rho_{L}}{2\pi\varepsilon_{0}}\int_{4}^{7}\frac{x-2}{(x-2)^{2}+16}dx$
### 상기 값을 고려 해서 V를 구하여라
+ ### $V_{+}$ 과 $V_{-}$ 의 식이 유사 하기 때문에 적분 구간을 다음과 같이 일반화 하여 적분을 구한 후 각각의 값을 적용
  ### $\int_{4}^{7}\frac{x-6}{(x-6)^{2}+16}dx,\int_{4}^{7}\frac{x-2}{(x-2)^{2}+16}dx \ \longrightarrow \ \int_{4}^{7}\frac{x-a}{(x-a)^{2}+16}dx$
+ ### $u=(x-a)^{2}+16, du=2(x-a)dx, \quad x=4 \to u_{1}=(4-a)^{2}+16, \quad x=7 \to u_{2}=(7-a)^{2}+16$
  ### $I(a)=\int_{4}^{7}\frac{x-a}{(x-a)^{2}+16}dx=\int_{u_{1}}^{u_{2}}\frac{1}{2u}du=\frac{1}{2}ln|u|_{u _{1}}^{u _{2}} =\frac{1}{2}(ln|u _{2}|-ln|u _{1}|)=\frac{1}{2}ln|\frac{u _{2}}{u _{1}}|=\frac{1}{2}ln|\frac{(7-a)^{2}+16}{(4-a)^{2}+16}|$
+ ### $I(6)=\frac{1}{2}ln\frac{17}{20},I(2)=\frac{1}{2}ln\frac{41}{20}, \quad V=V_{+}+V_{-}=\frac{\rho_{L}}{2\pi\varepsilon_{0}}(-I(6)+I(2))=frac{\rho_{L}}{2\pi\varepsilon_{0}}\frac{1}{2}(ln\frac{41}{20}-ln\frac{17}{20})=\frac{\rho_{L}}{2\pi\varepsilon_{0}}ln\frac{41}{17}$
