---
Asignatura: Estructuras de datos y laboratorio
Tipo: Conceptual
Completo: true
Unidad: Unidad 1
Fecha: 2023-08-29
---

Es una relación entre el número de [[Buckets]] ocupados por datos y el espacio total libre que se tiene para mapear registros. 

Load Factor

$$Lf = \frac{n}{(m\times Bkfr)}$$
Siendo,

- $n$ el número de [[Registros]] mapeados en disco.
- $m$ el número de [[Buckets]] que se reservaron para mapear archivos.
- $Bkfr$ el factor de bucket con el que estamos trabajando.