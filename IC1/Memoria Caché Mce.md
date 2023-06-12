
Es una #Memoria auxiliar que se introduce entre el procesador (CPU) 
y la memoria principal (Mp)
- Es una memoria pequeña y rápida

[[Arquitectura Von Newman]]

## Propiedades
**Localidad de referencia**: Se puede predecir las instrucciones y datos que el programa utilizará a partir del conocimiento reciente de los accesos realizados a la Mp
	- Localidad temporal: Las palabras accedidas recientemente tienen una alta probabilidad de ser llamadas de nuevo
	- Localidad espacial: Las palabras próximas tienen una alta probabilidad de ser llamadas de nuevo

## Funcionamiento Mce
![[MceFuncionamiento.png]]

## Formas de organizar la Mce (Función de correspondencia)
La Mce es mas pequeña que la Mp en todos los casos

### 1. Correspondencia Directa

-  ==Se organiza por bloques==
- Cada bloque tiene su misma posición en la Mp, cuando se acaban los bloques en la Mce, se vuelve al inicio y se sobre escribe la información
- Opera realizando comparación simultanea de su contenido con el campo de etiqueta de la dirección física
### 2. Correspondencia Asociativa
- Los bloques de la Mp se alojan en cualquier bloque de la Mce, comprobando solamente la etiqueta. 

### 3. Correspondencia Asociativa por conjuntos
- Las líneas de Mce se agrupan por conjuntos

![[MceFuncionDeCorrespondencia.png]]



# Tasa de aciertos y de fallos

#### Acierto de cache (hit)
El contenido de la dirección se encuentra  en un bloque ubicado en una linea de la caché
#### Fallo de caché (miss):
El contenido no se encuentra en ningún bloque de la Mce

# Algoritmos de sustitución
- **Aleatoria**: Se escoge un bloque al azar
- **LRU (Least Recently Used)**: Se sustituye el bloque que hace más tiempo no ha sido referenciado
- **[[FIFO]]**: Se sustituye el bloque que ha estado más tiempo en Mce (se puede implementar con una cola)
- **LFU (Least Frequently Used)**: Se sustituye el bloque que ha experimentado menos referencias (Se puede implementar asociando un contador a cada marco de bloque)

## Política de escritura
Es la forma de actualizar la Mp cuando se realizan operaciones de escritura hay dos casos
1. Cuando la posición de memoria sobre la que se va a escribir ==está== en Mce ==ACIERTO==.
2. Cuando ==No está== es un ==FALLO==.

- **Escritura directa o inmediata**: Todas las operaciones se realizan en Mp y Mce, es más lento, hay que poner un buffer
- **Postescritura (copy back)**: Actualizaciones solo en Mce, se utiliza un bit asociado al bloque para indicar la escritura del marco en Mp (genera inconsistencia temporal complica el acceso de la E/S)
- **Asignación en escritura (write allocate)**: El bloque se ubica en Mce cuando ocurre un fallo y se opera como un acierto
- **No asignación en escritura (No write allocate)**: El bloque se modifica en Mp sin cargarse en Mce

## Política de búsqueda
- **Por demanda**
- **Anticipativa**

## Clasificación de fallos

- Forzosos: producidos por el primer acceso a un bloque 
- Capacidad: producidos cuando Mce no puede contener todos los bloques del programa 
- Conflicto: (en correspondencia directa o asociativa por conjuntos) producidos por la necesidad de ubicar un bloque en un conjunto lleno cuando Mce no está completa.
