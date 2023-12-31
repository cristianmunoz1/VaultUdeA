---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: true
Unidad: Unidad 3
Tema general: Distribuciones de variables aleatorias discretas
---
Si $X$ es una [[Variable aleatoria discreta]] con una distribución Bernoulli, entonces, su distribución de probabilidad está dada por:

$$P(X=x)=\left\{\begin{array}{cc}
p^x(1-p)^{1-x} & x=0,1 \\
0 & \text { en otro caso }
\end{array}\right.$$
$E[X]=\mu = p$

$V[X]=\sigma^2=p(1-p)$



Cuando trabajamos con estas distribuciones, siempre vamos a etiquetar los casos de 2 posibles formas. **Éxito** o **fracaso**, dependiendo de cual es mi objetivo y qué es lo que estoy analizando. Y se realiza el experimento **una sola vez**. 

Si analizamos la función de masa de probabilidad que definimos anteriormente, podemos hallar que:

- $p^x$ es la [[Probabilidad]] de éxito
- $(1-p)$ es la [[Probabilidad]] de fracaso
### Ejemplo
Quiero lanzar una moneda, y encontrar la **probabilidad** de que salga **cara**. Cuando salga cara, lo tomaremos entonces como un **éxito**, y cuando salga sello como un **fracaso**. Adicional a esto, al éxito le pondremos el valor de 1 y al fracaso de 0.

$P(X=1)=\left(\frac{1}{2}\right)^1\times \left(1-\frac{1}{2}\right)^{1-1}=\frac{1}{2}$

$P(X=0)=\left(\frac{1}{2}\right)^0\times \left(1-\frac{1}{2}\right)^{1-0}=\frac{1}{2}$
