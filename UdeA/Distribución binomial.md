---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: 
Unidad: Unidad 3
---
La distribución binomial es una generalización de la [[Distribución Bernoulli]]. Igualmente se estudiarán experimentos dicotómicos. Pero se puede realizar el experimento $n$ veces.

La distribución binomial modela la [[Probabilidad]] de los resultados de un [[Experimento]] así:

- Tiene $n$ ensayos individuales, independientes.
- Cada ensayo tiene sólo 2 resultados posibles: éxito o fracaso (ensayo Bernoulli)
- Cada ensayo tiene una [[Probabilidad]] de éxito $p$ y es constante. 
- Aplicaciones: Inspección de calidad, ventas, mercadotécnia, medicina, investigación de opiniones, entre otras. 

**Variable de interés:**
$X$: número de éxitos obtenidos en los $n$ ensayos. 

**Rango:**
$A_X=\{0,1,2,...,n\}$

- Si $X$ tiene una distribución binomial con parámetros $p$ y $n$, su función de probabilidad es:
$$P(X=x)=p(x)=\binom{n}{x}p^x(1-p)^{n-x}$$

### Media y varianza de una distribución binomial

Sea $X$ $\textasciitilde{}$ $Binom(n,p):$

#### Media:
$E[X]=np$

#### Varianza:
$Var[X]=np(1-p)$
 


