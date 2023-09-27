---
Asignatura: Estructuras de datos y laboratorio
Tipo: Conceptual
Completo: true
Unidad: Unidad 1
Fecha: 2023-09-07
---

Esta técnica nos permite resolver colisiones al momento de hacer hashing estático y soluciona el problema planteado cuando usamos [[Encadenamiento]].
Lo que debemos hacer es un [[Encadenamiento]], pero a cada registro con diferente resultado de la función de direccionamiento lo mapeamos en un espacio en disco reservado exclusivo para él y sus sinónimos que generen colisiones. Ligamos el espacio en disco con el [[Área de overflow]] reservada para dicha "familia de registros".