---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: true
Unidad: Unidad 3
Tema general: Distribuciones de variables aleatorias discretas
---
Primero, identifiquemos con qué tipo de [[Experimento]] podemos resolver problemas usando la Distribución hipergeométrica. 

- Una urna contiene 6 bolas rojas y 14 amarillas, 5 bolas son extraídas sin reemplazamiento. ¿Cual es la probabilidad de que exactamente 4 bolas sean extraídas?. Cualquier muestra de 5 bolas tiene la misma probabilidad de salir. 
- **Solución: **
$$\frac{\text{Número de casos favorables}}{\text{Número de casos totales}}$$

$$\frac{\binom{6}{4}\cdot \binom{14}{1}}{\binom{20}{5}}$$

### Experimento hipergeométrico

Suponga que una población finita tiene $N$ elementos, cada uno de los cuales tiene una de dos características diferentes (por ejemplo, $K$ elementos tienen la característica de interés y $N-K$ no la tienen). Se toman al azar y sin reemplazo $n$ de estos elementos. 

Urna con:
- $N$ elementos en total
- $K$ elementos de interés
- $N-K$ no son de interés
- $n$ elementos seleccionados


La **Distribución hipergeométrica** modela la probabilidad de los resultados de un experimento así:

- Se tiene una población finita de $N$ elementos.
- Se tienen $k$ éxitos y $N-k$ fracasos.
- Se toman (extraen, eligen) al azar y sin reemplazo $n$ de los $N$ elementos. 
- Cada elemento tiene solo 2 características posibles: Éxito o fracaso (Ensayo Bernoulli).
- Por lo tanto, $p$, (la probabilidad de éxito) no es constante y los ensayos no son independientes. 

### Variable de interés

$X$, el número de elementos que tienen la misma característica de interés en los $n$ elementos seleccionados.

**Rango**, los valores que toma esta variable aleatoria son: $x=0, 1, 2, min(n,K)$


### Construcción de la f.m.p de $X$

$\binom{N}{n}$, que es la forma de seleccionar $n$ objetos de $N$.

$\binom{K}{x}$, formas distintas de seleccionar $x$ elementos de los $K$

$\binom{N-K}{n-x}$, formas distintas de seleccionar $(n-x)$ de los $(N-K)$

Entonces, la [[Función de masa de probabilidad]] de $X$, está dada por:

$$P_X(x)=\left\{\begin{array}{cc}
\frac{\binom{K}{x}\cdot \binom{N-K}{n-x}}{\binom{N}{n}} & x=0,1,2,..., min(n, K) \\
0 & \text { en otro caso }
\end{array}\right.$$

### Media de una distribución hipergeométrica

Sea $X\sim Hiper(N, K, n)$, entonces:

$$E[X]=n\frac{K}{N}$$

### Varianza de una distribución hipergeométrica

Sea $X\sim Hiper(N, K, n)$, entonces:
$$Var[X]=\left(\frac{N-n}{N-1}\right)\cdot n\cdot \frac{K}{N}\cdot \left(1-\frac{K}{N}\right)$$
