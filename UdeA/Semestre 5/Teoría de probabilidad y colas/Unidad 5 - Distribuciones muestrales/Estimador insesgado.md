---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: 
Unidad: Unidad 5
Fecha: 2023-10-11
---
El [[Estimador]] puntual $\widehat{\theta}$ es un estimador insesgado o centrado en el parámetro $\theta$ si la esperanza matemática del estimador $\widehat{\theta}$ es igual al parámetro $\theta$, esto es:
$$E(\widehat{\theta})=\theta, \ \text{Entonces, }\ E(\widehat{\theta})-\theta=0$$

En otro caso, decimos que es sesgado. Si $\widehat{\theta}$ es sesgado, el sesgo se define como:
$$\beta=E(\widehat{\theta})-\theta$$

Donde $\beta$ es conocido como sesgo del estimador $\widehat{\theta}$.



#### Para el [[Promedio de la media muestral]] y la [[Varianza de la media muestral]]

Sea $X_1, \ ...\ , X_n$ una muestra aleatoria de una distribución con media $\mu$ y varianza $\sigma^2$, entonces $\overline{X}$ y $S^2_{n-1}$ son estimadores insesgados para $\mu$ y $\sigma^2$, respectivamente. 

- Ya conocimos el resultado $E[\overline{X}]=\mu$

- También puede mostrarse que $E[S^2_{n-1}]=\sigma^2$


# Estimador insesgado de la varianza mínima

Cuando estemos frente a varios estimadores no sesgados, (centrados en el valor real del parámetro), y debamos escoger uno con el cual hacer las estimaciones, el que más nos conviene sería el estimador con menos varianza de todos, porque está más cercano, o tiene todos los valores mucho más cercanos al parámetro $\theta$ por lo tanto, nos puede proporcionar una mejor estimación. 