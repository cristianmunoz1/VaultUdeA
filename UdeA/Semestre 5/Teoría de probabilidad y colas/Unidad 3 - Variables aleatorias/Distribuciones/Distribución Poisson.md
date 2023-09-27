---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: true
Unidad: Unidad 3
Tema general: Distribuciones de variables aleatorias discretas
---
Esta distribución modela experimentos de el siguiente tipo:

- Número de errores tipográficos por páginas
- Número de llamadas telefónicas a una central por minuto
- Número de baches por kilómetro en una vía
- Número de accidentes en un cruce por una hora
- Número de bacterias en un cultivo

Osea, son conteos dependiendo de un tiempo, volúmen, o medición que nos interese para el [[Experimento]]

- Interesa hacer un conteo del número de veces que ocurre un evento por unidad de tiempo o espacio.
- En cada unidad de tiempo o de espacio, el número de eventos que ocurre es independiente de los que ocurren en otras unidades.
- La probabilidad de que un evento ocurra es la misma para todas las unidades de un mismo tipo.

### Variable de interés
$X$: Número de eventos que suceden a una tasa $\lambda$ (sobre tiempo o espacio).
$\lambda$ para nosotros, será una tasa de ocurrencia. (En los problemas se dará)

### Rango
El rango es abierto pero discreto

$$A_X=\{0,1,2,...\}$$

### Función de masa de probabilidad
$$P(X=x)=p(x)=\frac{\lambda^xe^{-\lambda}}{x!}$$
$$0, \text{En cualquier otro caso}$$

### Media de una distribución Poisson

Sea $X\sim P(\lambda)$

$$E[X]=\lambda$$
Es decir, el parámetro $\lambda$ corresponde al número promedio de ocurrencia del evento por unidad de tiempo o espacio. 

### Varianza de una distribución Poisson

$$Var[X]=\lambda$$

### Características
- La tasa de ocurrencia promedio $\lambda$ es constante.
- La probabilidad de que suceda un evento es proporcional al tamaño del intervalo de tiempo y espacio considerado.
- Dos eventos no pueden ocurrir exactamente al mismo tiempo o en el mismo punto del espacio.  

