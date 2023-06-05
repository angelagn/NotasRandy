Para implementar: [[Secuencia Implementar]]
1. Es una [[Colección]] que funciona como las colas en la vida real, es una estructura tipo [[FIFO]]
[[Estructura Lineal]]
2. Son secuencias a las que se accede por dos puntos
3. Su semántica implica un #RecorridoDestructivo, no se puede recorrer sin destruirla
4. Requiere mucha memoria

## Características
>- Incorpora datos al final de la #Cola 
>- Hay que recorrer de la cabeza a la cola
>- La cola se puede generar a partir de una [[Lista Enlazada]] uniendo los nodos del principio al final por medio de punteros y ya funcionarían con toda la lógica y operaciones de estas listas
>- NO permite acceso aleatorio
>- Solo se accede al principio o al final o ambos

## Operaciones

### Encolar
>- Insertar al final **enqueue()**

### Procesar / consultar
>- Obtener el siguiente elemento de la cola
>- Ver que se tiene en la cabeza de la lista o cola y no hacer nada **getFirst()**

### Eliminar
>- Eliminar la cabeza **dequeue()**
>- Echar el siguiente elemento de la cola una vez ha sido eliminado

![[Cola o Stack.png]]

## Optimizaciones
>- Poner punteros a la cabeza y final de la #Cola 
>- #Despachar Para despachar hay que seguir tres pasos:
>- - Extraer el primer elemento
>- - Eliminarlo
>- -Devolverlo para que se procese}

## Interfaz

![[QueueIF1.png]]
![[QueueIF2.png]]