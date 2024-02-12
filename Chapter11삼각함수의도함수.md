## Background-1

### $\lim_{x \to 0} \frac{\text{sin}x}{x}=1$증명하라
+ ### 라디안 : 반지름과 호의 길이의 비, 1 라디안 : 반지름(r) = 호의 길이 (라디안은 비율이기 때문에 원의 크기에 상관없이 적용)
+ ### 원주율($\pi$) : 원의 지름(d)에 대한 둘레(l)의 비율,  $\pi=\frac{\text{l}}{\text{d}}=\frac{\text{l}}{\text{2r}}, 2\pi r=\text{l}$
+ ### 부채꼴의 넓이 : $\frac{1}{2}r^{2}\theta$
+ ### 반지름이 1인 원에서 넓이에 대해 다음이 성립 된다.
![geogebra-export](https://github.com/DooHub/Electromagnetic_Math/assets/99073912/406ad945-29ae-48b5-b646-e0173c8b154c)

  ### 삼각형ABC넓이 < 부채꼴ABD넓이 < 삼각형AED넓이 $\longrightarrow \frac{1}{2}\times 1 \times \text{sin}x\lt \frac{1}{2} \times 1^{2}\times x \lt \frac{1}{2} \times 1 \times \text{tan}x$
  ### $\frac{2}{\text{sin}x}$을 곱해주면 $1\lt \frac{x}{\text{sin}x}\lt \frac{1}{\text{cos}x}$
  ### 1보다 큰수의 역수는 1보다 작고 0보다는 크다. $\quad 1\gt \frac{\text{sin}x}{x}\gt \text{cos}x \gt0, \quad \lim_{x \to 0} \text{cos}x=1\quad \therefore \frac{\text{sin}x}{x}=1$
## Background-2
### $\lim_{x \to 0} \frac{\text{cos}x-1}{x}=0$증명하라
+ ### $\lim_{x \to 0} \frac{\text{cos}x-1}{x}=\lim_{x \to 0} \frac{(\text{cos}x-1)(\text{cos}x+1)}{x(\text{cos}x+1)}=\lim_{x \to 0} \frac{\text{cos}^{2}x-1}{x(\text{cos}x+1)}=\lim_{x \to 0} \frac{-\text{sin}^{2}x}{x(\text{cos}x+1)}$
### $\qquad \qquad \qquad \quad \ =\lim_{x \to 0}\frac{\text{sin}x}{x}\frac{-\text{sin}x}{\text{cos}x+1}, \quad \lim_{x \to 0}\frac{\text{sin}x}{x}=1,\lim_{x \to 0}\frac{-\text{sin}x}{\text{cos}x+1}=\frac{0}{2}=0 \quad \therefore 1 \times \frac{0}{2}=0$
