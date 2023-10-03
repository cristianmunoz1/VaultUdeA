---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: false
Unidad: Unidad 3
Fecha de clase: 2023-09-25
Tema general: Variables aleatorias
---
Siempre que los ensayos binomiales sean demasiado grandes y la probabilidad de éxito se encuentre al rededor de $\frac{1}{2}$, una distribución binomial si observamos su gráfica podemos observar un parecido a una normal. Esto nos da una idea de que usando la [[Distribución normal]] podemos aproximar una [[Distribución binomial]]. 

Para que la aproximación de la binomial con la normal sea correcta (Ya que la binomial es discreta y la normal es contínua) debemos hacer una corrección por continuidad. Es común usar un factor de corrección, usualmente $\frac{1}{2}$

![[Figura 14.png]]
*Se puede observar la forma parecida a una distribución normal*

Dependiendo de como se relacione el número de ensayos con la probabilidad de éxito, la forma de la binomial será cada vez más parecida a una normal. 

Entonces,

Sea $X\sim Binom(n,o)$ para $n$ grande, se tiene que:

$$P(X\leq x)=P\left(X\leq x +\frac{1}{2}\right) \approx P\left(Z\leq \frac{x+\frac{1}{2}-np}{\sqrt{np(1-p)}}\right)$$

$$P(X\geq x)=P\left(X\geq x - \frac{1}{2}\right)\approx P\left(Z\geq \frac{x-\frac{1}{2}-np}{\sqrt{np(1-p)}}\right)$$

(Para que contenga al punto $x$)

$$P(a\leq X\leq b)=P\left(a-\frac{1}{2}\leq X\leq b+\frac{1}{2}\right)\approx P \left(\frac{a-\frac{1}{2}-np}{\sqrt{np(1-p)}}\leq Z \leq \frac{b+\frac{1}{2}-np}{\sqrt{np(1-p)}}\right)$$

**¿Cómo podemos saber si se le suma o se le resta el factor de corrección?**
Se debe tener muy presente cuando vamos a aplicar el factor de corrección si estamos trabajando con $\leq, \geq$ o con $<, >$. De eso depende la manera de aplicar el factor de corrección. Por lo tanto, cuando trabajemos con intervalos inclusivos, debemos sumarlo. Si no es inclusivo, lo restamos. 

**¿Cuando son buenas estas aproximaciones?**
En la práctica, las aproximaciones son buenas cuando $np\geq 10$ y $n(1-p)\geq 10$

Cuando cualquiera de estas 2 verificaciones no cumpla, debemos graficar la distribución binomial para observar que la forma de esta se acerque a una normal. 

