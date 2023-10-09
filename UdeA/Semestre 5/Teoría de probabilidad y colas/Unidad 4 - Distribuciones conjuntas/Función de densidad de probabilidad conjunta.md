---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: 
Unidad: Unidad 4
Fecha: 2023-09-29
Tema general: Distribuciones conjuntas
---
Sean $X$ y $Y$ dos variables aleatorias contínuas. Para un conjunto $A$ en 2 dimensiones, la probabilidad se calcula con función de densidad de probabilidad conjunta (f.d.p.c) para cualquier conjunto $A$ en 2 dimensiones así:

$$\begin{gather*}P(X, Y \in A)=\iint_{A} f(x,y)\,dx\, dy \end{gather*}$$

Es la integral doble de la función de densidad $f(x,y)$


### Propiedades

- $f(x,y)\geq 0$

- $\int_x \int_y f(x,y)dydx=1$

- $F(x,y)=P(X\leq x,Y\leq y)=\int_{-\infty}^x \int_{-\infty}^y f(x,y)dy\, dx$


Entonces, para cualquier conjunto $A$ en 2 dimensiones

$$P\lbrack(X,Y)\in A\rbrack = \iint_{A}f(x,y) \, dx \, dy$$

En particular, si $A$ es el rectángulo bidimensional $\{(x,y):a\leq x\leq b\, ,c\leq y\leq d)\}$, entonces

$$P\lbrack(X,Y)\in A\rbrack=P(a\leq x\leq b\, , \, c\leq y\leq d)=\int_{a}^b \int_c^d f(x,y)\, dy \, dx$$



### Distribuciones marginales

Cuando nosotros queremos saber cual es la función de densidad de probabilidad para una de las 2 variables aleatorias en concreto, a eso lo llamamos *Distribución marginal*

**Distribución marginal de $Y$**

$$f(y)=\int_x f(x,y)\, dx$$

**Dsitribución marginal de $X$**

$$f(x)=\int_y f(x,y)\, dy$$



### Distribuciones condicionales

También, cuando tenemos información adicional, lo que podemos hacer es calcular la probabilidad condicional, de la siguiente manera:

**Distribución condicional de $Y$ dado $X=x$**

$$f_{Y|x}(y)=\frac{f(x,y)}{f(x)}$$

**Distribución condicional de $X$ dado $Y=y$**

$$f_{X|y}(x)=\frac{f(x,y)}{f(y)}$$

---

Si deseamos encontrar la probabilidad de que la variable aleatoria $X$ caiga entre a y b cuando sabemos que la variable $Y=y$ , evaluamos

$$P(a<X<b \left|  Y=y\right.)=\int_{a}^{b}f_{X|y}(x)\, dx$$

---

Si $F$, (La acumulada) es contínua en $\mathbb R^2$, existe una función

$$f:\mathbb{R}^2\rightarrow \mathbb R^2$$
tal que:

$$\frac{\partial ^2F(x,y)}{\partial x\partial y}=f(x,y) \text{ donde exista la derivada.}$$


---
