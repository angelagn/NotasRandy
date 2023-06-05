
[[Estructura Lineal]] de tipo [[LIFO]] [[Colección]] Para implementar: [[Secuencia Implementar]]
- Acceso por un único punto -> cima
- no se puede modificar la cima porque implica borrar mas insertar
- #RecorridoDestructivo 

## Operaciones

### Apilar (push)
>- Introducir algo en la pila
>- Los elementos se introducen por un extremo
>- Se puede reutilizar la funcion Insertar
>-  Pila vacia = nodo vacío = #Null 

### Cima (peek)

>- El ultimo elemento en la cima es el ultimo en entrar
>- LA cima se obtiene buscando la cabeza de la lista

### Desapilar (pop) eliminar
>- Eliminar es sacar un elemento de la pila
>- Es descabezar la pila
>- La pila no puede ser vacia


### Otras operaciones

1. Comprobar: si la pila está vacía
2. Tamaño
3. Implementar como array
4. Desbordamiento:  El puntero ya no apunta al #Arrays , es un error [[Stack Overflow]] que hay que reportar
5. get top, muestra el ultimo elemento de la pila pero no lo toca

![[StackIF1.png]]
![[StackIF2.png]]