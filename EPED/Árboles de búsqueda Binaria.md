Es un árbol binario muy extendido es una [[Estructura Jerárquica]]  de tipo [[Colección]] 
Es un árbol especializado en realizar búsquedas de datos **ORDENADOS**


### Condiciones
1. Todos los mayores que la raíz en un hijo
2. Todos los elementos menores que la raíz en otro hijo
3. LO anterior se debe cumplir para todos los #subarboles 

## Elementos comparables

Un árbol de búsqueda puede almacenar elementos que cumplan una relación de orden
1. debe haber una forma de ordenar elementos ej: Alicia > Benito


## Estructura recursiva
1. #Nodo  a la vez va a ser árbol y puede o no tener #subarboles 
2. el árbol vacío va a ser #Null 

## Operaciones

### Búsqueda
- Igual que la raíz  -> encontrado
- Mayor que la raíz -> Buscar en hijo de elementos mayores
- Menor que la raíz -> Buscar en hijo de elementos menores
 
 ![[Arbol busqueda.png]]

Preguntamos si 
X == R?
1. X == R -> Ya encontramos el elemento en la propia raíz
2. X < R    -> Buscar en  subarbol izquierdo
3.  X > R   -> Buscar en subarbol derecho donde están los elementos mayores


### Insertar
 Introducir un elemento de forma ordenada
 Distinguir si el árbol permite duplicados o no 
 NO PERMITIR MODIFICAR EL ÁRBOL DESDE AFUERA PORQUE ES MUY COSTOSO CONSULTAR DESDE AFURA
#### Reglas
1. Si el árbol vacío, entonces insertar en raíz
2. SI raíz == al elemento a insertar? Si el árbol no permite duplicados, no se inserta o se emite un error [[Exception]]
3. Si la raíz es mayor al elemento a insertar? Insertar en subarbol izquierdo
4. si la raíz es menor al elemento a insertar? Insertar en subarbol derecho

Insertar: (a: Arbol, elemento: k)

#Puntero Cuidado al conectar los punteros, verificar que funcionan

### Eliminar
1. Buscar el nodo
La eliminación depende  de:
1. Si el nodo a almacenar es #Hoja : Se elimina el nodo y se hace que el puntero ahora apunte a #Null 
2. Eliminar nodo con 1 #Hijo : Reemplazamos la raiz por la raiz del nodo hijo, el padre del nodo a eliminar ahora debe apuntar al hijo del nodo a eliminar
3. Eliminar nodo con 2 hijos: NO se puede perder la info de los hijos, a la vez se debe reestructurar el arbol. Hay que promover a alguno de los nodos hijo como raiz

>- Nodo más a la derecha del subarbol izquierdo = nodo con el valor máximo dentro del subarbol izquierdo
>- Nodo más a la izquierda del subarbol derecho = nodo con el valor mínimo dentro del subarbol derecho

![[BSTreeIF1.png]]
![[BSTreeIF2.png]]
