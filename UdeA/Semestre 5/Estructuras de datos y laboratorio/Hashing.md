---
Asignatura: Estructuras de datos y laboratorio
Unidad: Unidad 1
Completo: true
Fecha de clase: 2023-09-04
---


Es una técnica pensada para llegar de manera muy rápida y eficiente a una ubicación en el disco donde se encuentren los [[Registros]] específicos que nosotros estemos consultando. 

Trabaja con una función matemática y un número m de [[Buckets]] reservados en el disco.

La función es la siguiente:
$$F(X_i)=I$$

Donde $X_i$ es un valor de clave de un registro.

Donde $I$ se mueve en el rango de 0 a m.

Y donde $I$ es el valor del bucket donde se va a almacenar el registro en el disco. 

Con esto claro, vamos a algunas definiciones importantes:

### Definiciones

- **Factor de bucket** (Bkfr): Es el número de registros que se pueden mapear en un bucket.
- **Factor de carga**: (Lf): Es la proporción entre el número de registros mapeados y el espacio total en disco. $Lf = n/(m \times Bkfr)$
- **Sinónimos**: Dados $X_i$ y $X_j$  con $X_i\neq X_j$ , se dice que son sinónimos si $F(X_i)= F(X_j)$   
- **Colisión**: Denominamos colisión al sinónimo $Bkfr + i$   con   $i>0$. En otras palabras, estamos tratando de insertar más registros de los que se pueden en un bucket.


### Recomendaciones para la función de transformación
La función de transformación $f()$ debe:
- Hacer una dispersión uniforme de las claves en todo el rango. Que no sea sesgada, osea, que no tienda a llevar todos los registros a un mismo bucket.
- Operar sobre todo el dominio. 

### Tipos de hashing
- [[Hashing estático]]
- [[Hashing dinámico]]
