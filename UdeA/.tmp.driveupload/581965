---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: true
Unidad: Unidad 3
Tema general: Variables aleatorias contínuas
---
La función de distribución acumulada para una [[Variable aleatoria contínua]] $X$ es la probabilidad de que $X$ tome un valor menor o igual a $x$, es decir:
$$F_X(x)=P(X\leq x) = \int_{-\infty}^{x}f_Y(y)dy$$

#### Propiedades:

- $$0\leq F_X(x)\leq 1,   \forall _X \in \mathbb R$$
- $$\lim_{x\to -\infty}F_X(x)=0$$
- $$\lim_{x\to \infty} F_X(x)=1$$
- $$P(a\leq X \leq b)=P(a\leq X < b)=P(a<X\leq b)=P(a<X<b)$$
$$=F_X(b)-F_X(a)$$

- $$P(X>a)=1 -P(X\leq a)=1-F_X(a)$$
Podemos observar que la función de distribución acumulada es una [[Función contínua]] contínua y una [[Función monótona creciente]]. 


#### Ejemplo:
Sea $X$ una variable aleatoria contínua.

1. Determine el valor de $k$ de tal manera que la siguiente función sea una [[Función de densidad de probabilidad]]:
$$f_X(x)=\left\{\begin{array}{l}
kx^2, \text { si } -1\leq x\leq 1 \\
0, \text { en otro caso. }
\end{array}\right.$$
2. Determine la [[Función de distribución acumulada v.a.c]] de $X$ y grafíquela.
3. Calcular $P(X\geq \frac{1}{2})$ y $P(-\frac{1}{2}\leq X \leq \frac{1}{2})$

#### Solución:
1. Siempre que tengamos un problema con un $k$ en la función de masa de probabilidad vamos a utilizar la propiedades que nos dice:
$$\int_{-\infty}^{\infty}f_X(x)dx=1$$
	Por lo tanto, tenemos: 
	$$\int_{-\infty}^{-1}0dx+\int_{-1}^{1}kx^2dx+\int_{1}^{\infty}0dx=1$$

$$k\int_{-1}^{1}x^2dx=k\left[\frac{x^3}{3}\right]_{-1}^1$$
$$\frac{k}{3}[1+1]=\frac{2}{3}k = 1$$
$$k=\frac{3}{2}$$

Por lo tanto, la [[Función de densidad de probabilidad]] queda entonces de la siguiente manera:
$$f_X(x)=\left\{\begin{array}{l}
\frac{3}{2}x^2, \text { si } -1\leq x\leq 1 \\
0, \text { en otro caso. }
\end{array}\right.$$

2. Sabemos que por definición, la [[Función de distribución acumulada v.a.c]] es la [[Probabilidad]] de que la variable aleatoria $X$ tome valores por debajo de $x$. También, sabemos que la podemos hallar calculando la integral de la [[Función de densidad de probabilidad]] de la siguiente manera:
$$F_X(x)=P(X\leq x)=\int_{-\infty}^{x}f_Y(y)dy=\int_{-\infty}^{-1}0dy+\int_{-1}^{x}\frac{3}{2}y^2dy$$
$$\frac{3}{2}\times \left[\frac{y^3}{3}\right]_{-1}^x = \frac{1}{2}\left[x^3+1\right], -1\leq x\leq 1$$


$$F_X(x)=\left\{\begin{array}{l}
0, \text { si x}< -1, \\
\frac{1}{2}(x^3+1), \text { si . } -1\leq x \leq 1, \\
1, \text{ si x} >1
\end{array}\right.$$

**Gráficamente:**
![[Figura 3.png]]

3. Como sabemos que la [[Función de densidad de probabilidad]] se mueve solamente entre $-1$ y $1$, lo que hacemos es partir la integral de la siguiente manera:
	Sabemos que por definición:
	$$P(X\geq \frac{1}{2})=\int_{\frac{1}{2}}^{\infty}f_X(x)dx=\int_{\frac{1}{2}}^{1}\frac{3}{2}x^2dx+\int_{1}^{\infty}0dx$$
	$$=\frac{3}{2}\times \left[\frac{x^3}{3}\right]_\frac{1}{2}^1=\frac{1}{2}\left[1-\frac{1}{8}\right]=\frac{7}{16}$$
	Ahora para calcular $P(-\frac{1}{2}\leq X \leq \frac{1}{2})$ lo hacemos de la siguiente manera:
	$$P(-\frac{1}{2}\leq X \leq \frac{1}{2})=\int_{-\frac{1}{2}}^{\frac{1}{2}}\frac{3}{2}x^2dx=\frac{3}{2}\left[\frac{x^3}{3}\right]_{-\frac{1}{2}}^\frac{1}{2}=\frac{1}{2}\left[\frac{1}{8}+\frac{1}{8}\right]=\frac{1}{8}$$
	