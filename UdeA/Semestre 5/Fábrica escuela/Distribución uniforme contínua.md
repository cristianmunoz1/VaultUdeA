---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: 
Unidad: Unidad 3
Fecha de clase: 2023-09-02
Tema general: Distribuciones de variables aleatorias contínuas
---
La variable aleatoria $X$ tiene una distribución uniforme contínua sobre el intervalo $[a, b]$ si su [[Función de densidad de probabilidad]] está dada por:

$$f(x; a,b)=\left\{\begin{array}{cc}\frac{1}{b-a}   \text{    Si a }\leq x \leq b \\ 0 \text{  en otro caso}\end{array}\right.$$

- Se dice entonces que $X\sim U_{[a,b]}$
- Todos los valores de $X$ dentro de $[a, b]$ son equiprobables.

![[Figura 9.png]]

La [[Función de distribución acumulada v.a.c]] la podemos calcular de la siguiente manera:

$$F_X=\left\{\begin{array}{cc}\frac{x-a}{b-a}\text{ Si }a\leq x\leq b \\ 0, \text{ En otro caso} \end{array} \right.$$


Sea $X\sim U_{[a,b]}$:

$$E[X]=\frac{a+b}{2}$$
$$V[X]=\frac{(b-a)^2}{12}$$
