---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: true
Unidad: Unidad 3
---
Sea $g(X)$ = $(X-\mu_X)^2$, la varianza de $X$, denotada como $Var[X]$ o $\sigma_X^2$ o $\sigma^2$, se define así:
$$Var[X]=E[(X-\mu_X)^2]=E[X^2]-(E[X])^2$$

Es una [[Medida de dispersión]]. Y con ella podemos calcular que tan separados están los datos unos de otros. Sin embargo, no es correcto extraer conclusiones desde la varianza, y es más acertado realizarlo desde la [[Desviación estándar (v.a)]]. 


### Propiedades

- $Var[a]=0$

- $Var[a^2\cdot X+b]=a^2\cdot Var[X]$

- La raíz cuadrara de $Var[X]$ se llama [[Desviación estándar (v.a)]]. Se denota como  $\sigma$


### Ejemplo
Sea $X$ una variable aleatoria que representa el número de clientes que llega a una tienda en un período de una hora. Dada la siguiente información:

| $x$    | 0      | 1      | 2      | 3      | 4      | 5      | 6      | 7      | 8   |
| ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | --- |
| $p(x)$ | $0.05$ | $0.10$ | $0.10$ | $0.10$ | $0.20$ | $0.25$ | $0.10$ | $0.05$ | $0.05$    |

Hallar el valor esperado y la varianza de la variable aleatoria.

#### Solución:

Analizando la tabla podemos encontrar que la información que nos presentan es una variable aleatoria la cual indica el número de clientes que llega a una tienda en una hora. Y a cada uno de estas cantidades de clientes, se les asigna una probabilidad. 

Hallemos el [[Valor esperado]]:

$E[X]=\sum_{x=0}^{8}x\cdot p(x)$

$$=(0)\cdot (0.05)+(1)\cdot (0.10) + (2)\cdot(0.10)+(3)\cdot(0.10)+ \\
(4)\cdot(0.20)+(5)\cdot(0.25)+...$$
$$...(6)\cdot(0.10)+(7)\cdot(0.05)+(8)\cdot(0.05)$$
$$=4$$
Eso nos dice que el promedio de clientes que llegan en un periodo de una hora es de $4$.

Hallemos la [[Varianza (v.a)]]:

$V[X]=E[x^2]-\mu ^2$

Debemos encontrar el dato $E[x^2]$

$E[X^2]=\sum_{x=0}^{8}x^2\cdot p(x)$

$$=(0)^2\cdot (0.05)+(1)^2\cdot (0.10) + (2)^2\cdot(0.10)+(3)^2\cdot(0.10)+ \\
(4)^2\cdot(0.20)+(5)^2\cdot(0.25)+...$$
$$...(6)^2\cdot(0.10)+(7)^2\cdot(0.05)+(8)^2\cdot(0.05)$$

$$=20.1$$
Ya con este dato podemos calcular la varianza:

$V[X]=E[X^2]-\mu^2=20.1-(4^2)=20,1-16=4,1$

Con esto, ya podemos calcular la [[Desviación estándar (v.a)]]:

$\sigma=\sqrt{Var[X]}=\sqrt{4,1}=2.025$
