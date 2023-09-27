---
Asignatura: Estructuras de datos y laboratorio
Tipo: Conceptual
Completo: true
Unidad: Unidad 2
Fecha: 2023-09-26
Tema general: Árboles
---

### Definición

Un árbol de búsqueda "M-Way" es un árbol en el cual todos los nodos son del grado $\leq M$ donde $M$ es su orden.
Si el árbol está vacío, es un árbol M-Way.
Cuando no está vacío tiene las siguientes propiedades:

- $T$ es un nodo del tipo:

| n   | $A_0$ | $(k_1, A_1)$ | $(k_2, A_2)$ | ... | $(k_n, A_n)$ |
| --- | ----- | ------------ | ------------ | --- | ------------ |


- Los $A_i$  $(0\leq i \leq n)$ son apuntadores a los subárboles del nodo $T$.

- Los $k_i$ $(1\leq i \leq n)$ son los valores de las claves. 

- $k_i<k_{i+1}$ con $(1\leq i \leq n-1)$

- Todos los valores de las claves en el subárbol $A_i$ son menores que la clave $k_{i+1}$

- Los subárboles $A_i$ son también árboles "M-Way". $(0\leq i\leq n)$


### Páginas

Cuando estamos creando árboles M-Way, tenemos un proceso el cual es agrupar nodos en bloques, a cada uno de estos bloques lo llamamos página.

Entonces, el tamaño de las páginas no puede ser arbitrario debido a que la memoria interna es limitada y también porque la lectura de una página demasiado grande toma mucho tiempo.

**¿Cual debe ser el tamaño de la página?**
Lo determina el tamaño del bloque. Queremos tener pequeños árboles de muy poco orden, para hacer la búsqueda más eficiente. 

### Búsqueda

Se busca en la raíz y se determina el valor de $i$ para el cual:

$K_i\leq x <k_{i+1}$

En el caso $X=k_i$ entonces la búsqueda es exitosa. 

Si es diferente, entonces por la definición de árbol M-Way $X$ debe estar en el subárbol $A_i$ si existe. 