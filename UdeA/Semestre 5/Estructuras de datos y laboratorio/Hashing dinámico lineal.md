---
Asignatura: Estructuras de datos y laboratorio
Tipo: Conceptual
Completo: 
Unidad: Unidad 1
---
Para realizar un hashing dinámico lineal debemos tener una [[Función]] en $k$ bits, y otra función en $k+1$ bits.
Supongamos que tenemos m [[Buckets]] reservados y un área de overflow. De la misma manera que se hace en [[Hashing estático]].

Su propósito es mantener el [[Factor de carga]] por debajo de un límite establecido. 

#### Paso a paso
Primero debemos realizar una búsqueda del bucket en el que vamos a insertar de la siguiente manera:

1. Calculamos la función de direccionamiento $f$ y asignamos los $k$ y $k+1$ bits a $f_k$ y $f_{k+1}$ respectivamente. 
2. Si $(f_k\geq lim)$ acceder al bucket $f_k$ sino, acceder al bucket $f_{k+1}$ 

Luego de la búsqueda, realizamos la inserción del registro de la siguiente manera:

1. Adicionamos el registro de la misma manera que en [[Hashing estático]]
2. Si $\frac{n}{m}>Lf\times Bkfr$, entonces adicionamos un bucket al área primaria $(m=m+1)$.
	1. Distribuímos el bucket límite entre él y el $m-1$ usando $k+1$ bits.
	2. Sumamos $1$ al límite. 
	3. Si límite es igual a $2^k$ entonces asignamos $0$ a límite y sumamos $1$ a $k$.