---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: 
Unidad: Unidad 3
Fecha de clase: 2023-09-20
Tema general: Distribuciones de variables aleatorias contínuas
---

Juega un papel clave en el desarrollo de la inferencia estadística, pues muchas de las herramientas usadas en la toma de decisiones o en el modelamiento estadístico, tienen su fundamento en esta distribución.

Un gran número de estudios pueden ser aproximados usando una distribución normal. Algunas variables físicas, datos meteorológicos, (Temperatura, precipitaciones, presión atmosférica, etc), mediciones en organismos vivos, notas o puntajes en pruebas de admisión o de aptitud, errores en instrumentación, proporciones de errores en diversos procesos, etc. 

Una [[Variable aleatoria contínua]] $X$ tiene una distribución normal si su [[Función de densidad de probabilidad]] es:
$$f(x, \mu, \sigma)=\frac{1}{\sigma \sqrt{2\pi}}e^{-\frac{1}{2}{\left(\frac{x-\mu}{\sigma}\right)^2}}, \text{ Si }-\infty\leq x\leq \infty$$

Donde $\mu \in \mathbb R$ y $\sigma > 0$, y se les conoce como parámetro de localización y escala respectivamente. 

A $\mu$ se le llama parámetro de localización porque como $\mu$ corresponde a la media, siempre será el pico de la curva, por lo tanto, su subimos $\mu$ entonces la curva se desplazará horizontalmente a la derecha para quedar con el centro o pico en $\mu$.

A $\sigma$ se le llama parámetro de escala porque nos modificará la curtosis de la curva, esto quiere decir, entre más alto sea este parámetro la curva tenderá a ser más achatada, o platicúrtica. En cambio, mientras más pequeño sea, la curva tenderá a ser leptocúrtica, las probabilidades se apilarán muchísimo más en un punto. Es una medida de dispersión. 

Se dice entonces que $X \sim N(\mu, \sigma^2)$

![[Pasted image 20230922120334.png]]


### Características

- El área bajo la curva Gaussiana entre $(-\infty, \infty)$ es igual a 1.
- La curva es simétrica respecto a $\mu$. El área bajo $[\mu, \infty)$ es 0.5
- La curva queda completamente caracterizada al conocer los parámetros de localización y escala
- Cuando más grande es $\sigma^2$, más achatada es la gráfica de la función.

### Media de una distribución normal

Sea $X\sim N(\mu, \sigma^2)$

$$E[X]=\mu$$

### Varianza de una distribución

Sea $X\sim N(\mu, \sigma^2)$

$$Var[X]=\mu$$

### Función de distribución acumulada

La obtenemos por medio de una [[Integral]]

Entonces si $X\sim N(\mu, \sigma^2)$, entonces la [[Función de densidad de probabilidad]] es: 

$$F_X(x)=P(X\leq x)=\int_{-\infty}^{x}\frac{1}{\sigma\cdot\sqrt{2\pi}}e^{-\frac{1}{2}\cdot\left(\frac{x-\mu}{\sigma}\right)^2}dx$$

Como podemos observar, esta integral no puede ser resuelta de manera explícita, y se deben usar métodos numéricos para aproximarla. Además, cada que se modifique alguno de los parámetros $\mu$ o $\sigma^2$, se debe calcular de nuevo dicha integral.

Para evitar este problema, se utiliza el cambio de variable $Z=\frac{x-\mu}{\sigma}$
Del cual se obtiene que $dz=\frac{1}{\sigma}dx$

Este cambio de variable se le conoce como **Estandarización**

De lo anterior se obtiene que:

$$\begin{aligned}
P\left(x_1<X<x_2\right) & =\int_{x_1}^{x_2} \frac{1}{\sqrt{2 \pi} \sigma} e^{-\frac{(x-\mu)^2}{2 \sigma^2}} d x \\ \\ \\
& =\int_{\frac{x_1-\mu}{\sigma}}^{\frac{x_2-\mu}{\sigma}} \frac{1}{\sqrt{2 \pi}} e^{-\frac{z^2}{2}} d z \\ \\ \\
& =P\left(z_1<Z<z_2\right)
\end{aligned}$$

De donde $z_1=\frac{x_1-\mu}{\sigma}$  y $z_2=\frac{x_2-\mu}{\sigma}$. Esto indica que cualquier cálculo de probabilidades para una variable aleatoria $N(\mu, \sigma)$ puede reducrise al cálculo de probabilidades con una variable aleatoria $N(0, 1)$. El proceso de transformar una variable aleatoria normal en una normal estándar se conoce como **Estandarización** o **Normalización**.


Observe que 

$$E[Z]=E\left[\frac{X-\mu}{\sigma}\right]=\frac{1}{\sigma}\cdot (E[X]-\mu)=\frac{1}{\sigma}(\mu-\mu)=0$$

$$V[Z]=V\left[\frac{X-\mu}{\sigma}\right]=\frac{1}{ \sigma^2}(V[X]-0)=\frac{1}{\sigma^2}(\sigma^2)=1$$


### En la práctica

En la práctica de la estandarización la haríamos como:

$$\begin{aligned}
P \left(x_1<X<x_2\right)& = P(x_1-\mu<X-\mu < x_2-\mu) \\ \\ \\
& =P\left(\frac{x_1-\mu}{\sigma}<\frac{X-\mu}{\sigma}<\frac{x_2-\mu}{\sigma}\right) \\ \\ \\
& = P(z_1<Z<z_2)
\end{aligned}
$$

### Función de distribución acumulada

Para el cálculo de probabilidades con una variable $N(0,1)$, la [[Función de distribución acumulada v.a.c]] estará dada por:

$$\phi(z)=P(Z\leq z)=\int_{-\infty}^{z}\frac{1}{\sqrt{2\pi}}\cdot e^{-\frac{z^2}{2}}dz$$

De esta manera se tiene que:

$$P(x_1<X<x_2)=P(z_1<Z<z_2)=\phi (z_2)-\phi(z_1)$$

**Densidad de la normal estándar** $N(\mu=0, \sigma^2=1)$

![[Pasted image 20230922202219.png]]

### Propiedades (simetría)

Sea $Z$ una variable aleatoria tal que $Z\sim N(0,1)$:

- $P(Z<-z)=P(Z>z)$

- $P(Z\geq -z)=P(Z\leq z)$

- $P(-z<Z<0)=P(0<Z<z)$

- $P(-z_1<Z<-z_2)=P(z_2<Z<z_1)$

- $P(-z\leq Z \leq z)=2P(Z\leq z)-1$

