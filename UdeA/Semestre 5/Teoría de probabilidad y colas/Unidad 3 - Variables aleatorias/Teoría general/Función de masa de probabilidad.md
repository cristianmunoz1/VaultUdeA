---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: true
Unidad: Unidad 3
Tema general: Variables aleatorias discretas
---
La función de masa de probabilidad de una [[Variable aleatoria discreta]] $X$ definida en un espacio muestral $S$, es una función matemática que asigna una [[Probabilidad]] a cada realización $x$ de la variable $X$. Se define así:

$$p(X)=P(X=x), \forall x \in X$$
Y podemos representar esta función de 3 maneras diferentes:
- Función
- Gráfica
- Tabla

### Propiedades
la función de masa de probabilidad satisface las siguientes propiedades:

- $p(x) \geq 0$ , $\forall x \in A_X$
- La sumatoria de todas las probabilidades da la unidad.
$$\sum_Xp(X)=1$$
- Si $A\subseteq A_X$, entonces:
$$P(X\in A)=\sum_{x\in A}p(x)$$


**Ejemplo de presentación en tabla:**
Tres monedas no cargadas son lanzadas simultáneamente. Continuando con el ejemplo inicial, se tiene interés en el número de caras que salen. Tabular la función de masa de probabilidad.

**Solución:**
El espacio muestral es el siguiente:
$$S=\{CCC, CCR, CRC, CRR, RCC, RCR, RRC, RRR\}$$

Por lo tanto, el rango de la función de masa de probabilidad es: 
$$A_X=\{0, 1, 2, 3\}$$

Calculamos la función de masa de probabilidad en cada uno de los valores del dominio: 

| x      | 0             | 1             | 2             | 3             |
| ------ | ------------- | ------------- | ------------- | ------------- |
| $p(x)$ | $\frac{1}{8}$ | $\frac{3}{8}$ | $\frac{3}{8}$ | $\frac{1}{8}$ |

