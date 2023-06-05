Los #Arboles son [[Estructura Jerárquica]] no lineales de tipo [[Colección]] en la que cada elemento puede preceder a ninguno, uno o más.
Puede existir una colección de árboles llamada bosque y también un árbol sin nodo llamado árbol vacío.
La forma de hacer operaciones depende de cada tipo de árbol [[Arboles Generales]]  [[Arboles binarios]]
[[Árboles de búsqueda Binaria]]


## Características

### Fan-out
No acotado, el árbol puede expandirse sin límite en anchura
### Distancia
Numero de elementos o saltos de un nodo a otro
### Altura de un elemento
Distancia de la raíz al elemento
### Altura del árbol
Distancia máxima de la raíz a la hoja
- _La altura de un árbol vacío es  -1_  
### Nivel 
Conjunto de nodos de un árbol a la misma altura 



>- Todo elemento es precedido por _un único elemento_
>- Cada nodo puede apuntar a otros nodos
>- Los datos van en cada #Nodo 
>- El árbol organiza los nodos
>- cada nodo puede apuntar a otros nodos y puede ser apuntado por otros nodos (generalmente)
>- Un #Nodo siempre va a ser a ser apuntado por un nodo llamado #Padre y apuntar simultáneamente a varios nodos llamados nodo #Hijo
>- Los árboles deben crecer en profundidad (en vertical) para eso se reduce el número de hijos

### Nodo Padre
padre de un elemento, su predecesor
### Nodo Hijo
Hijo de un elemento, cualquiera de sus sucesores
### Nodo Raíz
Elemento especial _Sin padres_ todos los demás nodos del árbol tendrán que tener un padre menos la raíz
### Nodo Hoja
El nodo #Hoja es un nodo que no tiene hijos, no se puede descender más por la jerarquía del árbol
### Hijo de un árbol
#subarboles   Un subárbol es cada nodo del que se desprenda un árbol


## Operaciones

- Obtener el elemento raíz
- Obtener el numero de hijos (arboles del árbol)
- Comprobar si el árbol es una hoja
- Obtener el fan-out del árbol
- Obtener la altura del árbol
- Obtener el iterador del árbol según el recorrido elegido

## Recorridos en profundidad

#Preorden ocurre cuando se visita a la raíz antes que a los hijos
![[ArbolRecorrido ProfundidadPreorden.png]]
#Postorden : Ocurre cuando se visita la raíz después de visitar a los hijos

![[ArbolRecorridoProfundidadPostorden.png]]

## Recorridos en anchura
- Se visitan los elementos por niveles, primero la raíz, luego los hijos de la raíz, luego los hijos de los hijos de la raíz y así.
![[ArbolRecorridoAnchura.png]]

## Propiedades de un árbol

 >- **Nivel**: A que distancia está un nodo del nodo raíz (medida en nodos)
 >- **Ruta**: Récord para hacer para avanzar de un nodo a otro 16 -> 24 -> 19 -> 21 
 >- **Altura | profundidad**: Máximo nivel que hay en un árbol hasta la hoja
 >- **Orden**: Indica cuantos nodos hijos puede tener cada nodo

### Orden
Es el número de hijos que puede tener cada nodo
>- Orden 2 -> 0, 1 o 2 hijos
>- Orden 3 -> 0, 1 o 2 hijos
>- Orden 4 -> 0, 1 o 2 hijos

Algunos ordenes tiene nombres especiales que definen tipos de árboles
>- Árbol binario -> de orden 2
>- Árbol terciario -> de orden 3

### Arbol Completo
Todos los nodos tienen: o cero hijos o el número máximo de hijos

![[Niveles de arbol.png]]


![[TreeIF1.png]]
![[TreeIF2.png]]



