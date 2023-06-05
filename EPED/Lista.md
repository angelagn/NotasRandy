Extiende de la clase [[Colección]] 
Para implementar: [[Secuencia Implementar]]
## Lista
Una #Lista es una [[Estructura Lineal]] que  son un tipo de [[Colección]] que hereda de la [[Interfaces]] collection, son una estructura de datos que respeta el orden en el cual fueron agregados los elementos, también permiten registros repetidos.
-  Especialización de la secuencia
- se accede y recorre los elementos, esto no destruye la lista

identifica:

>- Primer elemento
>- Último elemento

## Modelos de implementación
- Primero y resto: dame el primer elemento y el resto y luego el primer y el resto...
	- lista = lista vacía
	- lista = cabeza + resto (lista)
- Punto de interés: las acciones se realizan con base en el puntero
	- Puntero a una posición en la lista
	- insercion, acceso y modificación a través del punteo
- Acceso por posición: cada elemento tiene una posición el acceso se hace en esa posición, se inserta en esa posición
	- Consultar
	- Modificar elementos existentes
	- 

### Operaciones
>- Recorrer elemento
>- Insertar elemento
>- Eliminar elemento


### Insertar elementos en una lista
>- Lista vacía? el primer elemento es nulo, instanciar y asocial a nulo
>- Insertar al principio? (prepend) Nuevo nodo, el siguiente apunta al primero y luego se actualiza el primero.
>- Insertar al final? (append) BUscar el último, y apuntar al nuevo nodo
>- Insertar en la mitad? Recorrer la lista con el puntero que apunta al elmento anterior del que necesito. 

### Formas de recorrer una lista
La mejor forma de recorrer un lista es con un #Bucle, recorre los elementos del primero al úiltimo , el último elemento apunta a #Null para que finalice el [[Bucle]] , la lista se va recorriendo con puntero

### Eliminar elementos de una lista
>- Eliminar primer elemento:  generar una variable temporal para guardar el elemento ya que no se puede cambiar el elemento de valor, entonces se libera memoria con una variable temporal
>- Eliminar el último: Acceder al último elemento, guardarlo en variable temporal, usar el nodo para llegar al penúltimo elemento, cuando llegue a nulo, se extrae el siguiente a la variable temporal, se elimina el siguiente que tenga el penúltimo que es el nuevo último, eliminar variable temporal
>- Eliminar intermedio: Acceder a la posición anterior al elemento a eliminar, actualizar el puntero al siguiente del que quiero eliminar, eliminar de memoria


![[LIstIF.png]]
![[ListIF2.png]]
![[ListIF3.png]]

- No se puede eliminar, modificar ni obtener un elemento de una lista vacía

## [[Lista Enlazada]]

Es una #Estructura que permite representar un grupo de elementos en una secuencia
es diferente a los #Arrays 

Cuenta con un #Nodo cabeza y un #Puntero que apunta al siguiente nodo, en una lista enlazada, la #Cola es lo que no es cabeza de lista. Si la lista está vacía, la cola va a valer #Null , es decir que es el último elemento de la lista
Para accedder a un elemento de una lista hay que recoorer toda la estructura
![[Lista enlazada.png]]

## Estructura de la lista
1. Cabeza
2. Puntero a nodo
3. Fin estructura

### Ventajas
En general, las listas en comparación con los #Arrays  tienen las siguientes ventajas:

>- Pueden estar en cualquier posición de memoria
>- Son estructuras de longitud variable

### Desventajas

>- No tienen nocion de índice, por lo que no podemos hacer accesos aleatorios
>- Necesitan más espacio en memoria ya que necesitan almacenar los punteros

## Operaciones con listas

```python
ESTRUCTURA libro 
nombre = cadena[50] 
autor = cadena[50] 
isbn = cadena[10] 
FIN ESTRUCTURA

# lista de libros
ESTRUCTURA lista
cabeza = libro 
cola = puntero a lista 
FIN ESTRUCTURA

# guardar en una lista
ESTRUCTURA nodo
elemento = libro 
siguiente = puntero a nodo 
FIN ESTRUCTURA

ESTRUCTURA lista
cabeza = puntero a nodo 
FIN ESTRUCTURA

# crear un nodo
FUNCION   crearNodo(L: libro) : Nodo
Variable nuevoNodo :  Nodo 
nuevoNodo.Elemento = L 
nuevoNodo.Siguiente = Nulo # que no apunte a nada porque no sabemos a que apunta
DEVOLVER nuevoNodo
FIN FUNCION

# recorrer una lista
# empezando por el primer elemento y terminando por el último
# en java no hay punteros pero un objeto apunta a una posición de memoria
FUNCION   crearNodo(L: libro) : Nodo
Variable nuevoNodo :  Nodo 
nuevoNodo.Elemento = L 
nuevoNodo.Siguiente = Nulo # que no apunte a nada porque no sabemos a que apunta
DEVOLVER nuevoNodo
FIN FUNCION

FUNCION   RecorrerLista(L: lista)
Variable Puntero :  Nodo 
Puntero = L.cabeza 
MIENTRAS (Puntero != Nulo){
ProcesarElemento(Puntero.elemento)
Puntero = puntero.siguiente
}
FIN FUNCION
 ``