[[Ordenes de Complejidad]] [[Algoritmos]] [[Métricas de análisis]]

# Calcular el coste
- Definir el tamaño del problema
- Calcular el coste de cada una de las instrucciones

### Operaciones básicas
No dependen del tamaño del problema
- Operaciones entrada y salida
- Asignación
- Expresiones


![[CalcularCosteAlgoritmo.png]]


## Como sumar estos conjuntos
El coste de una secuencia de sentencias, viene marcado por el coste de la sentencia más costosa


![[ComposicionSecuencial.png]]

## Suma de ordenes
![[SumaDeOrdenes.png]]
### Producto de Ordenes
![[ProductoDeOrdenes.png]]

# Coste de #If
![[CosteDeIf.png]]
# Coste del #Switch

El máximo de todas las operaciones que hay que hacer

![[CosteDelSwitch.png]]

# Coste del #For [[Bucle]]
EL maximo entre calcular la inicializacion y multiplicar el numero de vueltas por el coste de calcular la expresion, el cuerpo del bucle y el incremento
![[CosteDelFor.png]]

# Coste del #While

![[Costedelwhile.png]]

# Coste del #DoWhile

![[CosteDelDoWhile.png]]

## Ej Coste de método
- tamaño del problema -> el vector
- entrada definida como la lognitud del vector n
- Decir el orden con respecto a que
![[EjCosteDeMetodo.png]]

# Coste de llamada a subprograma
![[CosteLlamadaASubprograma.png]]

## Reglas del calculo
### Recurrencias
La función del coste también es recursiva
y tiene dos formas
- Si n es un caso base la ==función== es:  T(n) = k```1(n)
- Si n no es caso base: a.T(n')+ k2(n)

==Resolver una recurrencia es dar una expresión no recursiva para T(n)==

- tamaño del problema se reduce mediante sustracción
- tamaño del problema se reduce mediante división

![[Resolucion RecurrenciaSustraccion.png]]
#RecursionSimple  o #RecursionLineal  es cuando solo hay una llamada recursiva, si a=1 y #RecursionMultiple cuando hay más de una llamada recursiva a>1

![[ResolucionRecurrenciasDivision.png]]