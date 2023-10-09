---
Asignatura: Teoría de probabilidad y colas
Tipo: Conceptual
Completo: 
Unidad: Unidad 4
Fecha: 2023-10-04
---
Esto se presenta cuando las variables aleatorias no influyen la una en la otra. Decimos que las variables son estadísticamente independientes. 

Sea $X$ y $Y$ dos variables aleatorias con una función de distribución conjunta $f(x,\ y)$, se dice que $X$ y $Y$ son estadísticamente independientes si y sólo si:

$$p(x, \ y)=p_X(x)p_Y(y) \ \ \text{Si X y Y son discretas}$$
$$f(x,\ y)=f_X(x)f_Y(y)\ \ \text{Si X y Y son contínuas}$$


Si al menos una pareja $(x, \ y)$ no cumple con lo anterior, se dice que $X$ y $Y$ son independientes. 


De esta manera, si $X$ y $Y$ variables aleatorias independientes, entonces:
*Para discretas:*

$$p_{X\ | \ Y}(x)=p_X(x)$$
$$p_{Y\ | \ X}(y)=p_Y(y)$$

*Para contínuas:*

$$f_{X\ | \ Y}(X)=f_X(x)$$
$$f_{Y\ | \ X}(y)=f_Y(y)$$



### Propiedades

Sean $a,\ b, \ c, \ d$, son constantes. Si $X$ y $Y$ son variables aleatorias independientes, entonces:

- $P(a <X<b, \ c<Y<d)=P(a<X<b)\cdot P(c<Y<d)$

- $E[XY]=E[X]\cdot E[Y]$

- $Cov[X, \ Y]=0$

- $\rho_{XY}=Corr[X, \ Y]=0$

**Nota:** Si $\rho_{XY}=0$, esto no implica que $X$ y $Y$ sean independientes. 

