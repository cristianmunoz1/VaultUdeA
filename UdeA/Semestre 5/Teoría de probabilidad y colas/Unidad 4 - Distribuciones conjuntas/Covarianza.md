---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: 
Unidad: Unidad 4
Fecha: 2023-10-04
---
Es una medida de variabilidad conjunta ([[Medidas de dependencia]]) que presentan 2 [[Variables aleatorias]]. La covarianza de $X$ y $Y$ se denota y se calcula así:

$$Cov(X, \ Y)=\sigma_{XY}=E[(X-\mu_X)(Y-\mu_Y)] = E[XY]-E[X]E[Y]$$

![[Pasted image 20231009114710.png]]


### Deducciones de la covarianza

- $\sigma_{XY}>0$   si valores grandes/pequeños de $X$ corresponden a valores grandes/pequeños de $Y$. *(Relación directamente proporcional)*

- $\sigma_{XY}<0$  si los valores grandes/pequeños de $X$ corresponden a valores pequeños/grandes de $Y$.  *(Relación inversamente proporcional)*

- $\sigma_{XY}=0$  no existe relación lineal. 

$$\begin{gathered}
\operatorname{Var}[a X+b Y]=a^2 \operatorname{Var}[X]-b^2 \operatorname{Var}[Y]+2 a b \operatorname{Cov}[X, Y] \\
\operatorname{Cov}[X, X]=\operatorname{Var}[X]
\end{gathered}$$



