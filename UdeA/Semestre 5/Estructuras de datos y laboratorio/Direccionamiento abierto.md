---
Asignatura: Estructuras de datos y laboratorio
Tipo: Conceptual
Completo: true
Unidad: Unidad 1
---

Este direccionamiento de los [[Registros]] en el disco para mapearlos, se realiza con un rehashing. 
Utilizamos una [[Función]] o una [[Familia de funciones]] para reubicar los [[Registros]] que generan colisión. 

Lo que nos dice el rehashing es que a la función que nos permite mapear los registros, le sumamos $i$ al resultado. 

**¿Qué ocurre si queremos borrar un registro?**
Cuando queremos borrar un registro bajo direccionamiento estático, lo que debemos hacer es un [[Borrado lógico]], los registros deben ocupar espacio desde el principio.

Cuando queramos buscar un objeto al que se le aplicó rehashing y ya existe un espacio en su bucket correspondiente porque hemos borrado un registro previamente, se mapea en el lugar donde aplicamos el borrado lógico. 

Lo anterior es una **Resolución lineal del problema**. Por lo tanto, podemos observar que cuando hay colisiones, los elementos tienden a agruparse en un solo punto, debido a que se utilizan los buckets siguientes más cercanos con espacios vacíos. 

Por lo tanto, sería mucho más eficiciente, debido a que dispersaría más los datos por los buckets, una **Resolución cuadrática** del problema. 

### Problema
Cuando el [[Factor de carga]] es muy alto, el desempeño de la aplicación se vuelve muy lento.

**¿Como se resolvería este problema?**
Primero, se debe pedir un espacio mucho más grande en disco. Debemos tener una función de direccionamiento completamente nueva y con esta función, procesar nuevamente registro por registro y mapearlo en el espacio nuevo con la función de direccionamiento nueva. 