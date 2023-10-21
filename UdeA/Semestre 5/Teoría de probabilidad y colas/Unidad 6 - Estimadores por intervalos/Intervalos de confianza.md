---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: 
Unidad: Unidad 6
Fecha: 2022-10-18
---
# Definición
Es un intervalo que obtenemos cuando observamos una muestra en el cual puede estar el parámetro real de la distribución que estamos estimando con cierto nivel de seguridad o de "Confianza". 
Los niveles de confianza más comunes son 90%, 95%, 99%.
Esto se interpreta como, que dentro de cada intervalo de confianza que calculemos, el valor del parámetro se encontrará allí con un % específico de seguridad. Esto significa, que si por ejemplo, sacamos 100 intervalos de confianza al 95%, en 95 de estos intervalos estará contenido el parámetro. 

Para calcularlos necesitamos un estimador puntual y conocer la distribución de muestreo.

Proporciona un [[Intervalos de números reales]] que contiene a $\theta$ con cierta seguridad. 

$$(L, \ U), \ \text{ donde } L<\theta<U$$

Si tomamos muchas muestras, cada una nos proporciona un valor diferente para $\theta ,\  L,\  U$ por lo que podemos observar que los extremos también son [[Variables aleatorias]].

$$(L, \ U)\ \text{ es un intervalo aleatorio.}$$

En este curso, trabajaremos intervalos de **confianza simétricos**


Si conocemos $\widehat{\theta}$ y su distribución de muestreo es posible calcular

$$P(L<\theta < U)=1-\alpha \ \text{ con } \alpha \in (0, \ 1)$$
$(L, \ U)$ se conoce como intervalo de confianza al $100(1-\alpha)\%$ para $\theta$

$L, \ U$ son los **límites de confianza.**

# Nivel de confianza
$(1-\alpha)\times 100\%$ indica que $(1-\alpha)\times 100\%$ de todas las muestras contienen el parámetro.

# Precisión
Longitud del intervalo de confianza. Entre mayor sea la longitud del intervalo más incertidumbre se tendrá sobre el valor estimado. 

# Relación entre nivel de confianza y precisión
Tienen una relación inversamente proporcional, debido a que una confianza del $100\%$ indica que el intervalo ocupa todo el ancho de los datos, por lo tanto la precisión será $0$. Y cuando haya más precisión, como el intervalo es más pequeño, tenemos menos posibilidades de que el valor estimado se encuentre dentro de dicho intervalo. 

Para alterar dicha relación, sacamos tamaños de muestra grandes, debido a que entre mayor sea la muestra, más nos aproximamos a la población. 

# Obtención del intervalo de confianza

$\widehat\theta$ es un estimador $f(x;\ \theta)$

$\widehat{\theta}=y(X_1, \ X_2, \ ..., \ X_n, \ \theta)$

Entonces, podemos encontrar constantes $a,\ b$ tales que

$$P(a<\widehat\theta<b)=1-\alpha$$
$$P(L<\widehat\theta<U)=1-\alpha$$
$$L=L(X_1, \ X_2,\ ...,\ X_n;\ a)$$
$$U=U(X_1, \ X_2,\ ...,\ X_n;\ b)$$
Para la muestra obtenemos $l=l(X_1, \ X_2,\ ...,\ X_n)$ y $u=u(X_1, \ X_2,\ ...,\ X_n)$

Armemos el intervalo de confianza para la media muestral. Para ello, usamos el siguiente diagrama de flujo. 
![[Pasted image 20231020200455.png]]

Podemos observar 4 casos principales y maneras de proceder para encontrar los intervalos de confianza de la media muestral. 

## Caso 1
Sea $X_1 ,\ X_2, \ ... ,X_n$ una muestra aleatoria que viene de una población **No normal**, con **n grande** y $\sigma ^2$ conocida. Hallamos $L$ y $U$ tales que el intervalo tenga una confianza del $100(1-\alpha)\%$ para $\mu$.
![[Pasted image 20231020200959.png]]

Debemos tratar de llevarlo a una normal estándar. Se llevará de la siguiente manera:
Si sabemos que:

$$P(L<\mu<U)=1-\alpha$$
$$=P(-L>-\mu>-U)$$
$$=P(-U<-\mu<-L)$$
Y estandarizamos
$$P\left(\frac{\overline{X}-U}{\frac{\sigma}{\sqrt{n}}}<\frac{\overline{X}-\mu}{\frac{\sigma}{\sqrt{n}}}<\frac{\overline{X}-L}{\frac{\sigma}{\sqrt{n}}}\right)$$

$$P(z_1<Z<z_2)$$

Donde

$$z_1=\frac{\overline{X}-U}{\frac{\sigma}{\sqrt{n}}}$$
$$z_2=\frac{\overline{X}-L}{\frac{\sigma}{\sqrt{n}}}$$

E introducimos una nueva notación![[Pasted image 20231020203954.png]]

Por lo tanto, $z_1=-z_{\frac{\alpha}{2}}$ , y $z_2=z_{\frac{\alpha}{2}}$

$$-z_{\frac{\alpha}{2}}=\frac{\overline{X}-U}{\frac{\sigma}{\sqrt{n}}}$$

$$z_{\frac{\alpha}{2}}=\frac{\overline{X}-L}{\frac{\sigma}{\sqrt{n}}}$$

Despejando $U$ y $L$ encontramos:

$$U=\overline X \ + \ z_{\frac{\alpha}{2}}\frac{\sigma}{\sqrt{n}}$$
$$L=\overline X \ - \ z_{\frac{\alpha}{2}}\frac{\sigma}{\sqrt{n}}$$
Por lo tanto, el intervalo de confianza para el caso 1 es:

$$\mu\in\left(\overline X \ - \ z_{\frac{\alpha}{2}}\frac{\sigma}{\sqrt{n}}, \ \text{ } \overline X \ + \ z_{\frac{\alpha}{2}}\frac{\sigma}{\sqrt{n}}\right)$$

$$\overline X\mp z_{\frac{\alpha}{2}}\times\frac{\sigma}{\sqrt{n}}$$


El valor de $z_{\frac{\alpha}{2}}\times\frac{\sigma}{\sqrt{n}}$ siempre es igual, por lo tanto, para obtener varios intervalos lo que hacemos es ir moviendo $\overline X$ con los valores que queramos calcular. 

### Tamaño de muestra
El tamaño de la muestra para que la media se encuentre alejada $\epsilon$ unidades de la media poblacional con una confianza de $1-\alpha$:
$$P(|\overline X-\mu|<\epsilon)=1-\alpha$$
De donde,

$$n=\left(\frac{z_{\frac{\alpha}{2}}\cdot \sigma}{\epsilon}\right)^2$$


## Caso 2

Es exactamente igual que el caso 1 solo que no conocemos $\sigma^2$

Por lo tanto, usamos $S$, que es la varianza muestral. 

$$\mu\in\left(\overline X-z_{\frac{\alpha}{2}}\cdot \frac{S}{\sqrt{n}}, \ \overline X+z_{\frac{\alpha}{2}}\cdot\frac{S}{\sqrt{n}}\right)$$

## Caso 3

Ahora sabemos que la población se distribuye como una normal y también conocemos $\sigma^2$

No nos importa el tamaño de la muestra en este caso

$$\overline X \mp z_{\frac{\alpha}{2}}\cdot \frac{\sigma}{\sqrt n}$$

## Caso 4

Sabemos que la población se distribuye normalmente, no conocemos $\sigma^2$ y tenemos un tamaño de muestra muy pequeño. Debido a esto último no podemos estandarizar. 

$$z=\frac{\overline X-\mu}{\frac{\sigma}{\sqrt n}} \to \ \text{ tiene otra distribución}$$

Si se reemplaza $\sigma$ por $S$, ahora hallaremos la variable $T$

**T-student**
$$T=\frac{\overline X-\mu}{\frac{S}{\sqrt n}}\sim t(n-1)$$

$T$ tiene una distribución T-student, que es similar a la normal pero con **Colas más pesadas.**

Mientras mayor sea nuestro número de muestra, t-student se aproxima cada vez más a una normal. 

Para una variable $T\sim t(v)$ la tabla reporta el cuantil superior
$$P(T>t(v))=\alpha$$

![[Pasted image 20231020221420.png]]

$$\overline X\mp t_{\frac{\alpha}{2}}(n-1)\cdot \frac{S}{\sqrt n}$$


# Intervalo de confianza para la proporción

Sea $X$ una [[Variables aleatorias]] $\sim$ $Binom(n, \ p)$ si $n$ es grande, el [[Teorema del límite central]] garantiza lo siguiente:

$$\frac{X-np}{\sqrt{np(1-p)}}\sim N(0,\ 1)$$

$\widehat{p}=\frac{X}{n}$ es un [[Estimador]] insesgado para $p$, entonces:

$$\frac{\widehat{p}-p}{\sqrt{\frac{\widehat p (1-\widehat p)}{n}}}$$

Sea $X_1, \ X_2, \ ..., \ X_n$ una muestra que viene de cierta población con $n$ grande. Hallemos $L$ y $U$ tales que el intervalo tenga una confianza $100(1-\alpha)\%$ para $p$:

$$P(L<p<U)=1-\alpha$$
$$P(z_1<Z<z_2)$$
$$-z_{\frac{\alpha}{2}}=z_1=\frac{\widehat p - U}{\sqrt{\frac{\widehat p (1-\widehat p)}{n}}}$$
$$z_{\frac{\alpha}{2}}=z_2=\frac{\widehat p - L}{\sqrt{\frac{\widehat p (1-\widehat p)}{n}}}$$

Despejando $L$ y $U$ obtenemos:

$$U=\widehat p \ + \ z_{\frac{\alpha}{2}}\sqrt{\frac{\widehat p (1-\widehat p)}{n}}$$
$$L=\widehat p \ - \ z_{\frac{\alpha}{2}}\sqrt{\frac{\widehat p (1-\widehat p)}{n}}$$

