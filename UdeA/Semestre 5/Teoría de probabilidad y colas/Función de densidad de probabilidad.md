---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: true
Unidad: Unidad 3
Tema general: Variables aleatorias contínuas
---
Sea $X$ una variable aleatoria contínua. La función de densidad de probabilidad (f.d.p) de $X$, representada por $f_X(x)$ es tal que:

- $f_X(x)\geq 0$,    $-\infty < x < \infty$
- Probabilidad del espacio muestral:
$$\int_{-\infty}^{\infty}f_X(x)dx=1$$
- La densidad representa la probabilidad relativa de tomar un valor en el intervalo $dx$.


Esta probabilidad, debido a que estamos trabajando con valores contínuos, no la trabajamos en valores puntuales sino en [[Intervalos de números reales]]

La [[Probabilidad]] de que la variable tome valores dentro de un intervalo está dada por la [[Integral]] de la densidad:
$$P(a\leq X\leq b)=P(a\leq X < b)=P(a<X\leq b)=P(a<X<b)$$
$$\int_{a}^{b}=f_X(x)dx$$

Note que la probabilidad del intervalo $a\leq X\leq b$ es el área acotada por la función de densidad y las rectas $X=a$ y $X=b$.

![[Pasted image 20230919194110.png]]
