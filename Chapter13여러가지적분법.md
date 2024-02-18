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
### $I=\int_{}^{}\frac{(\text{tan}^{-1} x)^2}{1+x^2}dx$ 구하라
+ ### $\text{tan}\theta=x, \ \longrightarrow \ \frac{d}{dx}(\text{tan}\theta)=\frac{d(\text{tan}\theta)}{d\theta}\frac{d\theta}{dx}=\text{sec}^{2}\theta \frac{d\theta}{dx} ,\ \frac{d}{dx}(\text{tan}\theta)=\frac{d}{dx}(x)=1, \ \therefore \text{sec}^{2}\theta \frac{d\theta}{dx}=1$
+ ### $\theta =\text{tan}^{-1}x,\ \longrightarrow \ \frac{d\theta}{dx}=\frac{d}{dx}(\text{tan}^{-1}x)=\frac{1}{\text{sec}^{2}\theta}=\text{cos}^{2}=\frac{1}{x^2+1}, \ d\theta=\frac{1}{x^2+1}dx$
+ ### $I=\int_{}^{}\frac{(\text{tan}^{-1} x)^2}{1+x^2}dx=\int_{}^{}\theta^2d\theta=\frac{1}{3}\theta^3+C=\frac{1}{3}(\text{tan}^{-1}x)^3+C$
