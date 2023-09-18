---
Asignatura: Matemáticas discretas I
Tipo: Conceptual
Unidad: Unidad 1
Completo: true
---


Estas reglas se dividen en 2 grupos: Básicas y complementarias.

### Básicas:

*RFP:* Regla de formación proposicional.
*fbf:* Fórmula bien formada.

**RFP1:** Cualquier forma declarativa simple es una fbf. *(Definición de forma declarativa simple)*
**RFP2:** Si $R$ es una fbf, entonces $\neg R$ es una fbf. *(Definición de forma declarativa negada)*
**RFP3:** Si $R$ y $S$ son fbfs, entonces $R\lor S$ es una fbf. *(Definición de forma declarativa disyuntiva)*
**RFP4:** Si $R$ es una fbf, entonces $(R)$ también es una fbf. *(Definición de forma declarativa agrupada)*

### Complementarias:

**RFP5:** Sean $R$ y $S$ fbfs, entonces la fórmula $R\land S$ es una fbf y se define como: $\neg(\neg R \lor \neg S)$
**RFP6:** Sean $R$ y $S$ fbfs, entonces la fórmula $R\rightarrow S$ es una fbf y se define como: $\neg R \lor S$
**RFP7:** Sean $R$ y $S$ fbfs, entonces la fórmula $R\leftrightarrow S$ es una fbf y se define como: $(R \rightarrow S)\land (S \rightarrow R)$
**RFP8:** Una secuencia de símbolos del alfabeto proposicional es una fbf si y sólo si, puede obtenerse de las anteriores reglas de formación. 