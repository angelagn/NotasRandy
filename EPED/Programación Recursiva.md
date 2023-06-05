Un objeto se contiene a si mismo

## Objetos recursivos

- Tiene una recursividad infinita
	- Ej fractales
	- Romanescu (verdura fractal)
	- Muñecas rusas (la versión interna es más simplificada
 
### Estructuras recursivas en [[Programación]]

- Grafo general 
	- [[Colección]] de objetos con relaciones entre ellos
- [[Árboles]]
	- Relaciones jerárquicas hasta llegar a nodos
- [[Lista]]
	- no son [[Estructuras de datos]] recursivas, pero se pueden pensar como recursivas (primer elemento y resto de la lista y así con cada elemento)


## Definiciones recursivas

- Deben tener una condición no recursiva para que la recursividad termine y se llegue a una solución, el programa espera a que llegue a esa condición no recursiva y empieza a hacer las llamadas hacia arriba desde la ultima no recursiva a la primera

	-  en la lista el caso no recursivo es vacía
	-  Árbol caso no recursivo es vacío
- Acercarnos al caso no recursivo de llama **Simplificación**

### Ejemplos

![[EjProgramacionRecursiva1.png]]


![[EjProgramacionRecursiva2.png]]

## Ventajas
- más natural para estructuras recursivas
- más declarativa que [[Bucle]] e [[Iteradores]], nos acerca mas al concepto de definición
- Sencillos de verificar