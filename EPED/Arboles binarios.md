Son una [[Colección]] de tipo [[Estructura Jerárquica]], son #Arboles  de orden 2, es decir que cada nodo puede tener como máximo dos hijos. y cada subarbol, el derecho y el izquierdo es considerado como un hijo

## Fan-out
 Al ser binario el máximo de anchura va a ser 2
 
## Operaciones
Se procesa todo el #subarboles hijo

### Recorridos en profundidad:
hasta llegar a las #Hoja 

>- En #Preorden : Se procesa primero la raíz, árbol izquierdo y árbol derecho
>-  En #Inorden : Se procesa árbol izquierdo, raíz, árbol derecho, en orden, devuelve los elementos ordenados
![[ArbolesBinariosRecorridoInorden.png]]
>-  En #Postorden :  Se procesa la raíz al final, izquierdo, derecho, raíz

### Recorridos en anchura
Procesar todos los elementos de un nivel y luego pasar al siguiente nivel, se hace con [[Colas]]
- Se recorren todos los nodos de **Izquierda a derecha**
- Se recorren todos los nodos de **derecha a izquierda**}
![[ArbolRecorridoAnchuraDaI.png]]
## Tipos

### Full Binary Tree
Todos los #Nodo s del árbol tienen
>- O ningún hijo (son hojas)
>- O sus 2 hijos

### Complete Binary Tree
El último nivel puede prescindir de alguno de sus hijos (el #Padre del #Nodo #Hoja  solo tiene un #Hijo )

![[Arboles binarios.png]]


## Arboles degenerados
Cada nodo solo tiene un hijo y se comporta como lista

## Arboles balanceados
Intenta mantener la profundidad de sus 2 #subarboles la menor posible, el balance del árbol hace que las operaciones sean más eficientes (balanceo o equilibrio)
Existen tipos de balanceo y se puede aprovechar el balanceo para usar una regla u otra .
Si el árbol es binario, la estructura se puede simplificar

## Operaciones

>- Inserción
>-  Eliminación
>-  Localización
>- Recorrido (hacer un procesado de cada nodo)

![[BTreeIF1.png]]
Hijo izquierdo
![[BTreeIF2.png]] 
Hijo Derecho
![[BTreeIF3.png]]
