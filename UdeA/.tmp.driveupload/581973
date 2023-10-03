---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: 
Unidad: Unidad 3
Fecha de clase: 2023-09-25
Tema general: Variables aleatorias
---
Tiene una relación muy estrecha con una [[Distribución Poisson]]. Debido a que con la Poisson, nosotros medíamos cantidad de casos de éxito en cierta unidad de medida. Con la Exponencial, calcularemos cuanto es esta medición hasta que nos encontremos con un caso de éxito. Como se distribuye la unidad en donde se mueve la Poisson. 

La variable aleatoria $X$ tiene una distribución exponencial si su función de densidad de probabilidad está dada por:

### Función de masa de probabilidad de una distribución exponencial

$$f(x ; \lambda)=\left\{\begin{array}{cc}
\lambda e^{-\lambda x} & \text { si } x>0 \\
0 & \text { en otro caso }
\end{array}\right.$$
- Se dice entonces que $X\sim Exp(\lambda)$
- Se emplea para modelar algunos tiempos de falla y el tiempo en líneas de espera. 

![[Figura 15.png]]

![[Figura 16.png]]
![[Figura 17.png]]

Podemos observar que la función es *Monótona decreciente* y *Asintótica respecto al eje x*



### Función de densidad de probabilidad de una distribución exponencial

Si $X\sim Exp(\lambda)$, entonces la función de distribución acumulada es:

$$F_X(x)=\left\{\begin{array}{cc}
0, & \text { si } x<0 \\
1-e^{-\lambda x}, & \text { Si } x\geq 0
\end{array}\right.$$

Sea $X\sim Exp(\lambda)$

### Valor esperado de una distribución exponencial

$$E[X]=\frac{1}{\lambda}$$

$$V[X]=\frac{1}{\lambda^2}$$

De aquí, podemos deducir que la desviación estándar coincide con la media o valor esperado. 


### Propiedad de la falta de memoria

Para una variable aleatoria exponencial $X$,

$$P(X<t_1+t_2 | X>t_1)=P(X<t_2)$$
Analizando esto, es, la probabilidad que pase un evento $t_2$ dado que ya pasó un evento anterior $t_1$, es la misma probabilidad del evento $t_2$. A la distribución no le importa lo que haya pasado antes, solo le importa lo actual. 
