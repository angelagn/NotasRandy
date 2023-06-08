Las secuencias heredan de [[Colección]]  
[[Lista]] [[Pilas]] [[Colas]]
## Secuencia
- Nodo que almacena
	- un valor 
	- puntero al siguiente nodo

## Se enecesita
- un nodo inicial

# Sequence es una clase [[TAD]]
- La estructura de datos es un NodeSequence que solo se puede utilizar en Secuencias como pilas, listas y colas.
- Es la que va a implementar la estructura de los nodos

![[Sequence<E>IMplementacion.png]]

## Clase interna nodos

- Getters, setters
- 2 constructores 
	- uno que pone el valor a null
	-  el que pone el siguiente valor a null
	- 

![[SecuenciaImplementarNodo.png]]

# Implementar el iterador de la secuencia
Esta clase se usa para recorrer secuencias y árbol

- Primer nodo de la clase secuencia
- hasNext comprobar antes del get, para saber que el nodo existe, realiza dos acciones. devuelve el valor del siguiente y avanza al próximo
Lo que hacemos en los [[Arboles]] es secuencializarlos,  dependiendo del recorrido que hayamos decidido utilizar, hay que crear una secuencia generalmente [[Colas]] luego se meten todos los nodos en el orden que lo vayamos recorriendo y el iterador del árbol sera el iterador de esa cola, de esa secuencia. 
Con esta clase NO es necesario implementar otra clase con iteratorIF, esta clase implementa el iterador



![[SecuenciaIterador.png]]


### Metodos auxiliares
Ojo que este getNext es de nodeSequence

![[SecuenciaImplementacionMetodosAux.png]]

## Constructores
 El [[Método Constructor]]  de una secuencia vacía, llama al constructor de una coleccion, tamaño=0
si la secuencia no está vacia, obtenemos el primer nodo, y  creamos un nodo con ese valor
- Si introducimos un numero menor que 1 devuelve el primer nodo
-  Si introducimos un numero mayor que el tamaño devuelve excepcion

![[SecuenciasImplementarConstructores.png]]

## Metodos clear y contains
métodos heredados de CollectionIF


![[SecuenciasClearYContains.png]]