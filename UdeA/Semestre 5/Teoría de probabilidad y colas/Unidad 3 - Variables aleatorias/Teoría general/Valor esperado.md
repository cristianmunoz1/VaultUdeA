---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: true
Unidad: Unidad 3
Tema general: Variables aleatorias
---
Sea $X$ una [[Variable aleatoria contínua]] o una [[Variable aleatoria discreta]] con [[Función de densidad de probabilidad]] o [[Función de masa de probabilidad]] $f_X(x)$ o $p(x)$, la esperanza de $X$, o el valor esperado de $X$, o el valor promedio de $X$, denotado como $E[X]$ se define así:

$$\mu = E[X]=\sum_{x}x\cdot p(x), \text{ si la variable aleatoria es discreta}$$
$$\mu = E[X]=\int_{-\infty}^{\infty}x\cdot f_X(x)dx, \text{ si la variable aleatoria es contínua}$$


- Es usualmente denotado como $\mu$ o $\mu_X$
- Cuando $E[X]<\infty$, se dice que la esperanza existe.
- No existe si la integral no converge a un valor finito. 

### Propiedades
*Las siguientes propiedades se cumplen tanto para [[Variable aleatoria discreta]] como para [[Variable aleatoria contínua]]*

*Sean $a$ y $b$ constantes, y $X$ una variable aleatoria*

- $E[a]=a$

- $E[a\cdot X + b]=E[a\cdot X]+E[b]=a\cdot E[X]+b$

- Si $g(x)$ es una función de $X$, entonces:
$$E[g(X)]=\sum_{x}g(x)p(x), \text{ si es variable aleatoria discreta}$$
$$E[g(X)]=\int_{-\infty}^{\infty}g(x)f_X(x)dx, \text{ si es variable aleatoria contínua}$$


