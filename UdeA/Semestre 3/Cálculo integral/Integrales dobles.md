---
Asignatura: Cálculo integral
Tipo: Conceptual
Completo:
---
Las integrales dobles son integrales iteradas. Por lo tanto, se hacen realizando primero una de ellas y luego la otra. 

***Por ejemplo:***
$$\int_{a}^b \int_{c}^d f(x, y)\ dy\ dx = \int_{a}^b \left[\int_{c}^{d} f(x, y)\ dy \right ]\ dx$$
Indica que primero se integra respecto a $y$ y a partir de $c$ hasta $d$, y luego respecto a $x$ desde $a$ hasta $b$.

$$\int_{c}^d \int_{a}^b f(x, y)\ dx\ dy = \int_{c}^d \left[\int_{a}^{b} f(x, y)\ dx \right ]\ dy$$

Significa que primero se integra respecto a $x$ (manteniendo fija a $y$) desde $x=a$  a  $x=b$  y después se integra la función resultante de $y$ respecto a $y$ de $y=c$ hasta $y=d$. Observe que siempre se trabaja desde adentro hacia afuera. 


### Teorema de Fubini
*Este teorema indica cuando se puede cambiar el orden de integración sin que se altere el resultado de la integral doble*

Si $f$ es contínua en el rectángulo $R=\{(x,y)| \ a \leq x \leq b,\ c\leq y \leq d\}$, entonces

$$\int_{R} f(x,y) \ dA = \int_{a}^b \int_{c}^d f(x,y) \ dy\ dx = \int_{c}^d \int_{a}^b f(x,y) \ dx\ dy$$


En términos generales, esto es cierto si se supone que $f$ está acotada sobre $R$, $f$ es discontínua sólo en un número finito de curvas suaves y las integrales iteradas existen. 

![[Pasted image 20231009081029.png]]

En el caso especial donde $f(x,\ y)$ se puede factorizar como el producto de una función de $x$ y una función de $y$, la integral doble de $f$ se puede escribir en una forma particularmente simple. Para ser específicos suponga que $f(x,\ y)=g(x)h(y)$ y $R=[a,\ b]\times [c, \ d]$. Entonces el teorema de Fubini da

$$\iint_R g(x)h(y)\ dA=\int_{a}^{b} g(x)\ dx \ \int_{c}^{d}h(y) \ dy$$

---

### Tipos de regiones

#### Región plana TIPO I

Se dice que una región plana $D$ es **tipo I** si yace entre las gráficas de 2 funciones contínuas de $x$, es decir

$$D=\{(x,\ y) \ | \ a\leq x \leq b,\ g_1(x)\leq y \leq g_2(x)\}$$
Donde $g_1$ y $g_2$ son contínuas en $[a, \ b]$
Podemos también expresarlo de la siguiente manera: La variable $x$ se mueve entre 2 constantes y la variable $y$ se mueve entre 2 funciones en términos de $x$.  
![[Pasted image 20231009082424.png]]

Cuando tenemos una región tipo I entonces el orden de las integrales y sus límites de integración son:
$$D=\{ (x,\ y) \ | \ a \leq x \leq b, \ g_1(x)\leq y \leq g_2(x)\}$$

entonces 
$$\iint_D f(x, \ y) dA = \int_{a}^{b}\int_{g_1(x)}^{g_2(x)} f(x,\ y) \ dy \ dx$$


#### Región plana TIPO II

Es una región donde ahora la variable $x$ se moverá entre funciones en términos de $y$. Se pueden expresar como:

$$D=\{(x,\ y) \ | \ c\leq y \leq d,\ h_1(y)\leq x \leq h_2(y)\}$$
![[Pasted image 20231009083528.png]]

El **Orden de integración** es entonces:

$$\iint_{D} f(x, \ y)\ dA = \int_{c}^{d} \int_{h_1(y)}^{h_2(y)} f(x, \ y) \ dx \ dy$$


#### Región plana expresada en AMBOS TIPOS

![[Pasted image 20231009084840.png]]

![[Pasted image 20231009084953.png]]



### Propiedades de las integrales dobles

- $\iint_{R} \ [f(x, \ y)+g(x, \ y)] \ dA = \iint_{R} f(x, \ y)\ dA + \iint_{R} g(x, \ y)\ dA$


- $\iint_{R} \ c \ f(x, \ y)\ dA = c\iint_{R} \ f(x, \ y)\ dA$,  donde $c$ es una constante


- $\iint_{D} \ f(x, \ y)\ dA = \iint_{D_1}f(x, \ y)\ dA + \iint_{D_2}f(x, \ y)\ dA$
