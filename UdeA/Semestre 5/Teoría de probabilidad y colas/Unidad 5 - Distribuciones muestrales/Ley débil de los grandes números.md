---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: 
Unidad: Unidad 5
Fecha: 2023-10-11
---
Sea $X_1,\ X_2,\ ...,\ X_n$ una [[Muestra aleatoria]] con [[Varianza (v.a)]] finita, entonces $\overline{X}_n\to_p \mu$, donde $\mu$ es la esperanza común de las variables aleatorias

*Cualquiera que sea $\varepsilon > 0$ se tiene que*

$$\lim_{n\to \infty}P\left(\left|\frac{X_1\ + \ X_2 \ + \ ...\ +\ X_n}{n}\ -\ \mu\ \right| \ \geq \varepsilon\right)=0$$
**Prueba:**
Desigualdad de Chebyshev


---

Recordando, el [[Valor esperado]] de la muestra aleatoria tiende al [[Valor esperado]] de la población. Por lo tanto, cuando hagamos esta resta, si la aproximación es muy buena, va a tender a cero, debido a que son parecidas o iguales en términos de valores esperados. 