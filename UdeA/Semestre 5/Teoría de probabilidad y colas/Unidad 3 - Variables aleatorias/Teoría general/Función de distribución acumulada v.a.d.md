---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: true
Unidad: Unidad 3
Tema general: Variables aleatorias discretas
---
Sea $X$ una variable aleatoria discreta con [[Función de masa de probabilidad]] $p(x)$. La función de distribución acumulada de $X$, se representan con $F_X(x)$ y se define como:
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

**Presentación tabular de la [[Función de masa de probabilidad]]:

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
![[Figura 1.png]]


### Propiedades

- $0\leq F(x)\leq 1$, porque $F(x)$ es una probabilidad.
- $P(X>x)=1-P(X\leq x)=1-F(x)$
- Si $X<Y \longrightarrow F(x)<F(y)$
- $P(X=a)=F(a)-F(a-1)$
- $P(a\leq X \leq b)=F(b)-F(a-1)$
- $P(a<X<b)=F(b-1)-F(a)$
- $P(a\leq b) = F(b-1)-F(a-1)$
- $P(a<X\leq b)=F(b)-F(a)$

---
### Ejemplo
Una urna contiene 4 bolas blancas y 3 bolas negras. Se extraen al azar y sin reemplazo 2 bolas de dicha urna. Sea $X$: número de bolas blancas en las 2 extraídas. Hallar la [[Función de masa de probabilidad]] y la [[Función de distribución acumulada v.a.d]] de $X$. Expresarla en forma de gráfica y en forma tabular. 

#### Solución:
Hallamos el rango de $X$:
$A_X=\{0,1,2\}$

Hallamos la [[Función de masa de probabilidad]]:
$p(0)=P(X=0)=P(N_1\cap N_2)=P(N_1)P(N_2 | N_1)=\frac{3}{7}\times \frac{2}{6}=\frac{1}{7}$

*Esto representa la función de masa en 0. También lo podemos interpretar como la [[Probabilidad]] de que salgan 0 bolas blancas en la extracción, por lo tanto es, la probabilidad de que salgan 2 negras.
También lo podemos ver como cual es la probabilidad de que la primera salga negra, por la probabilidad de que salga negra la segunda, dado que la primera fue negra*

$p(1)=P(X=1)=P(B_1N_2\cup N_1B_2)=P(B_1N_2)+P(N_1B_2)=\left(\frac{4}{7}\times \frac{3}{6}\right)+\left(\frac{3}{7}\times \frac{4}{6}\right)=\frac{4}{7}$

$p(2)=P(X=2)=P(B_1\cap B_2)=P(B_1)\times P(B_2)=P(B_1)\times P(B_2|B_1)=\left(\frac{4}{7}\times \frac{3}{6}\right)=\frac{2}{7}$


Hallamos la [[Función de distribución acumulada v.a.d]]:
$F(x)=\left\{\begin{array}{l}0, \text { si } x<0 \\ \frac{1}{7}, \text { si } 0 \leq x<1 \\ \frac{5}{7}, \text { si } 1 \leq x<2 \\ \frac{7}{7}, \text { si } x \geq 2\end{array}\right.$
