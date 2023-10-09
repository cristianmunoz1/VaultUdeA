---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: 
Unidad: Unidad 5
Fecha: 2023-10-09
---
Sean $X_1, X_2, ..., X_n$ una muestra aleatoria de una distribución con media $\mu$ y varianza $\sigma^2$

Sea $\overline{X}$ la media muestral (la cual depende de n), entonces cuando $n$ tiende a infinito, la distribución muestral de $\frac{\overline{X}-\mu}{\frac{\sigma}{\sqrt{n}}}$ es aproximadamente normal estándar. 


En lenguaje matemático:

$$\frac{\overline{X}-\mu}{\frac{\sigma}{\sqrt{n}}}\sim N(0, \ 1), \ n\to \infty$$

- Entre mayor sea $n$ mejor es la aproximación.
- Si la distribución muestral es simétrica y contínua, $n$ pequeño permite obtener buenas aproximaciones. 
- Si la distribución es discreta, se requiere $n$ grande


$\overline{X}$ es una variable aleatoria también. Por lo tanto, se puede calcular lo siguiente:

$$P(\overline{X}\leq a)\approx P\left(\frac{\overline{X-\mu}}{\frac{\sigma}{\sqrt{n}}}\leq\frac{a-\mu}{\frac{\sigma}{\sqrt{n}}}\right)$$

Si $\sigma^2$ es desconocida y $n$ es grande, se puede reemplazar a $\sigma^2$ por $S^2$. Así:

$$\frac{\overline{X}-\mu}{\frac{S}{\sqrt{n}}}n\to N(0, \ 1)$$

