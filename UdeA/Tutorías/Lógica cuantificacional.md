---
Asignatura: Matemáticas discretas I
Tipo: Tutoría
Completo: 
Unidad: Unidad 2
Fecha: 2023-09-29
Estudiante: Estefanía Garcés
---
**¿Por qué utilizamos el cálculo cuantificacional?**

Es una extensión del cálculo proposicional, que nace de la necesidad de contar usando el cálculo proposicional. 

### Alfabeto cuantificacional

#### Símbolos de constantes
$a, b, c,d,e$
Y les podemos agregar subíndices

#### Signos de variables
$u,v,w,x,y,z$
Y les podemos agregar subíndices

#### Signos de función
$f,g,h,i,j,k$
Se le puede agregar subíndices si hacen falta signos
$f_i, g_i, h_i, j_i, k_i$


$f(e, c)=e$
Una función señala un individuo que resulta de la relación entre 2 o más individuos. 


#### Signos de predicados
$l,m,n,o,p,q,r,s,t$
Se le puede agregar subíndices si hacen falta signos

$p(x):$ $x$ es una mujer.
$p(e):$ El objeto $e$ es una mujer. 

$q(x, y):$ $x$ es padre de $y$

#### Signo de cuantificador
$\forall:$  Cuantificador universal


### Reglas de formación cuantificacional

#### RFC1
Forma atómica, átomo, literal. Es un predicado con $n$ argumentos. 

$$p(t_1, t_2, t_3, ..., t_n)$$

	$t_i$ representa un individuo, se les denomina argumentos o términos. 
	Aridad: Cantidad de términos que tiene una forma atómica. 
	Cuando el predicado no tiene términos (p), se convierte en una fbf del cálculo proposicional.

Para los términos podemos usar constantes, variables, o funciones. 

#### RFP2
Definición de fbfs negadas. 

$$\neg p(t_1,t_2)$$
#### RFP3
Definición de fbfs disyuntivas

$$\lor$$

#### RFP4 
Definición de formas proposicionales agrupadas

$$()$$

#### RFC2
Definición de formas proposicionales universalmente cuantificadas

Si $R$ es una fbf y $x$ es una variable, entonces

$$\forall x R$$
es una fbf. 

### RFP5, RFP6, RFP7

### RFC3 
Definición de formas proposicionales existencialmente cuantificadas.

Si $P$ es una fbf del cálculo cuantificacional, entonces 
$$\exists xP$$ también es una fbf, y se define como:

$$\exists xP \iff \neg \forall x\neg P$$


### RFC4

Una secuencia de símbolos de este alfabeto es una fbf del cálculo cuantificacional si y solo si se obtiene de las anteriores reglas de formación. 


### Precedencia (jerarquía) entre las operaciones lógicas

$$\neg, \forall, \exists, \land, \lor, \rightarrow, ↔$$

Los 2 cuantificadores tienen el mismo orden de prioridad, sin embargo cuando se encuentre con dos símbolos de cuantificadores consecutivos, se aplica primero aquel que esté más a la derecha. 


## Otras definiciones básicas

#### Ámbito o alcance de un cuantificador
Lo conforman el símbolo de variable que lo acompaña  y la fbf más cercana que le sigue a la variable. 

![[Pasted image 20230929202412.png]]


#### Ocurrencia

Una ocurrencia de una variable $x$ es cada aparición de $x$.

#### Ocurrencia ligada o libre

Se dice que una variable $x$ tiene una ocurrencia ligada en una fbf $P$ si cae en el ámbito de algún cuantificador y coincide con el signo de variable que acompaña al cuantificador. De lo contrario se dice que su ocurrencia es **libre**. 


#### Fórmula bien formada libre de una variable

![[Pasted image 20230929205504.png]]

Se dice que la fbf P es libre de la variable 𝑥 si esta última no aparece en P, o si cada ocurrencia es ligada en P.


#### Fórmula bien formada cerrada
Si y solo si la fbf es libre de toda variable.

#### Fórmula bien formada abierta
Ai, y sólo si, no se encuentra libre de al menos una variable.


#### Particularización

$P_{x|t}$ es una fbf que se obtiene de la fbf P mediante el reemplazo de las ocurrencias libres de 𝑥 por un término 𝑡; a esta operación se le denomina *particularización*.


