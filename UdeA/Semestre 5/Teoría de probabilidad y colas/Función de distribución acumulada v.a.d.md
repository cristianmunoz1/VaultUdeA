---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: true
Unidad: Unidad 3
---
Sea $X$ una variable aleatoria discreta con función de masa de probabilidad $p(x)$. La función de distribución acumulada de $X$, se representan con $F_X(x)$ y se define como:
$$F_X(x)=P(X\leq x)=\sum_{x'\leq x}p(x')$$ $$\forall x \in \mathbb R$$
Además, podemos saber por esta función de qué tipo es la variable aleatoria que estemos tratando.
- Si $F_X(x)$ es una función escalonada, $X$ es una variable aleatoria discreta. 
- Si $F_X(x)$ es una función contínua, $X$ es una variable aleatoria contínua.
- Si $F_X(x)$ se puede expresar como una combinación lineal de funciones escalonadas y contínuas, $X$ es una variable aleatoria mixta. 

---
#### Ejemplo:
Tres monedas no cargadas son lanzadas simultáneamente. Escribir la función de distribución acumulada.

**Solución:** 
La variable aleatoria es $X$: número de caras obtenidas.
El rango de la variable es: $A_X={1,2,3}$

**Presentación tabular**:

| $x$    | 0   | 1   | 2   | 3   |
| ---- | --- | --- | --- | --- |
| $p(x)$ |  $\frac{1}{8}$   |  $\frac{3}{8}$   |  $\frac{3}{8}$   |  $\frac{1}{8}$   |

**Cálculo de la variable de distribución acumulada:**

$F(0)=P(X\leq 0)=P(X=0)=\frac{1}{8}$
$F(1)=P(X\leq 1)=P(X=0)+p(X=1)=\frac{1}{8}+\frac{3}{8}=\frac{4}{8}$
$F(2)=P(X\leq 2)=P(X=0)+p(X=1)+p(X=2)=\frac{1}{8}+\frac{3}{8}+\frac{3}{8}=\frac{7}{8}$
$F(3)=P(X\leq 3)=P(X=0)+p(X=1)+p(X=2)+p(X=3)=\frac{1}{8}+\frac{3}{8}+\frac{3}{8}+\frac{1}{8}=1$

**Presentación en función:**

$F(x)=\left\{\begin{array}{l}0, \text { si } x<0 \\ \frac{1}{8}, \text { si } 0 \leq x<1 \\ \frac{4}{8}, \text { si } 1 \leq x<2 \\ \frac{7}{8}, \text { si } 2 \leq x<3 \\ 1, \text { si } x \geq 3\end{array}\right.$

**Presentación en gráfica: **
![[Pasted image 20230918192909.png]]


### Propiedades

- $0\leq F(x)\leq 1$, porque $F(x)$ es una probabilidad.
- $P(X>x)=1-P(X\leq x)=1-F(x)$
- Si $X<Y \longrightarrow F(x)<F(y)$
- $P(X=a)=F(a)-F(a-1)$
- $P(a\leq X \leq b)=F(b)-F(a-1)$
- $P(a<X<b)=F(b-1)-F(a)$
- $P(a\leq b) = F(b-1)-F(a-1)$
- $P(a<X\leq b)=F(b)-F(a)$
