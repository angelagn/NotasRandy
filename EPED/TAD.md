**Un TAD es una colección de valores y de operaciones** definidos mediante una  **especificación independiente de cualquier representación**
Con mucha frecuencia se utilizan los términos _TDA_ y _Abstracción de Datos_ de manera equivalente, y esto es debido a la similitud e interdependencia de ambos.

La solidez de un TAD reposa en la idea de que la implementación está escondida al usuario. Solo la interfaz es pública.

## Abstracción de datos

La abstracción de datos consiste en ocultar las características de un objeto y obviarlas

>- Estructuras de datos y sus operaciones
>- Abstracción de datos, muestra las operaciones a realizar con los datos, pero oculta la implementación de las operaciones
>- Define un conjunto de operaciones que se pueden realizar con los datos
>- Son una herramienta fundamental en la [[POO]] ya que encapsulan los datos y las operaciones
>- Promueve la [[Modularización]] y rehuso de código
>- permite que los programadores se centren en el uso de los datos sin preocuparse por los detalles internos de implementación.
>- [[Colección]]

## Un TAD representa una abstracción
Sobre el que hace el programa y como lo hace. 

# La programación con TAD requiere dos pasos
1. ==Definición del tipo==: Decidir las operaciones necesarias para manipular los valores y especificarlas (tiene una parte sintáctica y otra semántica)
2. ==Implementación del tipo==: Elegir la representación de los valores e implementar las operaciones

#Encapsulación ES un concepto fundamental en la programación con TAD
	- **Privacidad** de la representación: el ususario no conoce los detalles
	- **Protección** del tipo: el usuario solo puede utilizar las operaciones previstas