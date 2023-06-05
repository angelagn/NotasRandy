[[Estructuras de datos]] [[Colección]]
## Que es la eficiencia de algoritmos


## Cómo se mide

- Gasto en memoria
- Tiempo empleado
- Otros recursos (ancho banda, consumo eléctrico...)
### Caso peor
los datos de entrada hacen que el algoritmo requiera mas tiempo, se mide por su coste **Asintotico** (cuando el tamaño de la entrada crece) **temporal** (porque estamos midiendo el tiempo  de ejecución ) **en el caso peor** (ante la entrada más costosa de procesar)
- El algoritmo va a consumir la máxima cantidad de recursos, para lo que se estima una cota superior de recursos

#### Como se analiza el coste:
- [[Métricas de análisis]]
	- Clasificación de funciones en familias
- Reglas practicas para medir la función de coste de un programa iterador ([[Iteradores]] ) como recursivo ([[Programación Recursiva]])

### Caso mejor
- El tiempo cuando los datos de entrada son óptimos

### Caso medio
- Distribución estadística de los casos de entrada, los casos más probables en los que se ejecutaría el algoritmo
