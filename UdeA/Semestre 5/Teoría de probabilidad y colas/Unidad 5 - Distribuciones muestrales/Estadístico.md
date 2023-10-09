---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: 
Unidad: Unidad 5
Fecha: 2023-10-09
---
Es una [[Función]] de la [[Muestra aleatoria]] que no tiene cantidades desconocidas.

- No todos los estadísticos de una m. a. son relevantes. 
- Existen algunos que permiten obtener aproximaciones a los parámetros de interés.


### Estadísticos de interés

Una buena aproximación para $\mu$ es:

$$\overline{X}=\frac{1}{n}\sum_{i=1}^n(X_i-\overline X)^2$$


Una buena aproximación para $\sigma^2$ es:

$$S^2=\frac{1}{n-1}\sum_{i=1}^{n}(X_i-\overline{X})^2$$


Una buena aproximación para $p$ es:

$$\frac{X}{n}, \ X\sim b(n, \ p)$$


Estadístico T:

$$T=\sum_{i=1}^{n}x_i$$
Y obtenemos que 
$$E[T]=n\mu$$$$ y $$
$$Var[T]=n\sigma^2$$

