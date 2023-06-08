- En la memoria se guardan datos o instrucciones de forma indistinta
- Ejecución secuencial salvo que
	-  un Condicional  #If  termina la secuencia
	- Interrupción
	- Acceso de [[Dispositivo de  Entrada-Salida]]


# Componentes básicos del sistema

- CPU
	- ALU: realiza operaciones básicas
	- UC: unidad de control (salen señales de control asociada a codigos de operacion)
	- Dos módulos (Registros)
		- MAR próxima dirección de memoria
		- MBR Contiene el dato a procesar
- Memoria principal
- Dispositivos E-S (tienen sus propios MAR y MBR )
	- teclado
	- mouse
	- impresora...


## Ciclo de instrucción 

Son ==Búsqueda== y ==ejecución==

- **Comienzo** (Cargar en el contador de programa la dirección donde inicia el programa)
- **Búsqueda** (ir a la posición y buscar todos los datos que necesitamos) Si se realiza acceso de memoria cuando se está busacndo la instrucción, el contenido que se encuentre será consideerado instrucción
- **Ejecucion** (Ejecuta la instruccion, y segun el resultado puede ir al acumulador o a la memoria o a la ALU o alterar la secuencia de ejecución) Si el acceso de memoria se realiza en estaa fase, lo que se ncuente srá considerado un dato
- **Parar**

## Ciclo de Interrupción

Al recibir una instrucción la CPU
- Guarda el Contador de Programa  (CP), datos y dirección de lo que estaba haciendo
- Carga en el CP instrucciones de inicio del programar de interrupción



## E/S -> CPU


## E/S -> Memoria
liberar a la CPU del proceso (DMA)

## E/S localizada en memoria
- 

# Estructuras de interconexion

## [[Bus]]
- Transportan tres cosas: ==Datos==, ==Direcciones== y ==Señales de Control==
-  Conectan 2 o más dispositivos
- Son compartidos, por diferentes dispositivos que pueden tener diferentes velocidades.

Bus de 8 bytes, lleva 8 cables
sistema de 64 bits... maneja 64 bits a la vez

## Ciclo de escritura
El tiempo de ciclo de escritura es la suma del tiempo de ocupación del #Bus más el tiempo de almacenamiento 


### Tipos de bus
Los buses son el embudo en la velocidad de los pc
La memoria principal está muy pegada a la CPU para que los datos lleguen más rápido

	**Bus de Datos**: Es el camino que se usa para  transferir entre módulos

	**Bus de Dirección**: camino desde donde seleccionamos una dirección de memoria o un dispositivo E/S, el dato que saque se va a través del bus de datos

	**Bus de Control**: Gobierna el uso y acceso a datos y direcciones 

### Lineas de Buses
- Dedicadas: Solo una función
- No dedicadas: Compartidas, varios elementos requieren sistema de arbitraje
- Para saber cuantas lineas de bus necesitamos según la cantidad de palabras, se saca el ==logaritmo en  base 2 de el numero de palabras==.


### Sistema de arbitraje: 
- Determina las prioridades del uso bus, se puede aumentar el nivel de prioridad
- Mientras la linea de bus ocupado esté activa, no se va a interrumpir el proceso así el nuevo tenga mayor prioridad

- **Centralizados**: 
	- El arbitro no sabe cuantos dispositivos hay
	- Solo puede saber si hay o no solicitudes
	- PRIORIDAD MÁS CERCANA AL ARBITRO
- **Distribuidos**
	- Igual, solo que no hay arbitro
	![[BusArbitrajeDistribuido.png]]

#### Técnica de multiplexación en el tiempo
Se comparten las mismas lineas de un #Bus para enviar daros o direcciones, es imposible mantener en paralelo una dirección y un dato #Multiplexado


# Temporización

- Los sistemas funcionan de una manera _Sincrona_ o _Asíncrona_
	- Bus con temporización _síncrona_:  Todos los dispositivos que se le conectan funcionan con una frecuencia de reloj fija. Su utilización es útil cuando ==***TODOS***== los dispositivos conectados tienen una velocidad de transferencia similar.
- Los + usados son forma asíncrona
- Oscilador (Reloj) , que oscila una frecuencia exacta F= 100MHz
- El ciclo es el periodo
- El periodo o ciclo es el inverso de la frecuencia 



## Puertas triestado

- Es un interruptor
- Indica que el driver está desconectado electricamente
-  NO hay ni 0 ni 1, el cable está desconectado electricamente
- Todas las puertas menos una, deben estar en estado de alta #Impedancia

## Velocidad de almacenamiento

Numero de palabras escritas en memoria por unidad de tiempo

### Velocidad de Transferencia
- 
- De dispositivos de E/S es la inversa del tiempo de ciclo (palabras por segundo)
	==Vt =1/ Tc==



