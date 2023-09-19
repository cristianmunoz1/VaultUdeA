---
Asignatura: Estructuras de datos y laboratorio
Tipo: Conceptual
Unidad: Unidad 1
Completo: true
---

Esta técnica para resolver las colisiones cuando usamos [[Hashing estático]] nos indica que, cuando haya una colisión, debemos pedir más espacio en disco, ([[Área de overflow]]) y conforme lleguen registros colisionados se mapearán de forma lineal en dicho espacio. 

### Problema
Cuando usamos esta técnica estamos mapeando registros con diferentes resultados de la función de direccionamiento a un mismo espacio lineal en disco, así que cuando tengamos muchos registros en el [[Área de overflow]] debemos recorrer cada uno de ellos hasta llegar al registro que queremos. Esto hace que mientras esta área sea más grande el rendimiento de la aplicación baje demasiado. 