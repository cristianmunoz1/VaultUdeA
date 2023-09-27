---
Asignatura: Estructuras de datos y laboratorio
Unidad: Unidad 1
Completo: true
Fecha: 2023-09-11
Tipo: Conceptual
---

Antes de definirlo, debemos saber, ¿Cual es una función que se mueve entre 0 y m?, siendo m el número de [[Buckets]] reservados en un disco. 

Tenemos la [[Función módulo]]. Con la que podemos obtener valores mayores e iguales a cero y menores que m, diviendo un número por m y obteniendo el residuo de la división. 

Otra función la podríamos hacer por una suma de una partición en k dígitos, y otra, eliminar los datos que produzcan un sesgo.

### Maneras de resolver colisiones
En hashing estático tenemos 3 diferentes formas de resolver este problema:

- [[Direccionamiento abierto]]
- [[Encadenamiento]]
- [[Encadenamiento separado]] 