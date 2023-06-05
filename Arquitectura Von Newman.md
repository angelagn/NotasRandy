- En la memoria se guardan datos o instrucciones de forma indistinta
- Ejecución secuencial salvo que
	-  un Condicional  #If  termina la secuencia
	- Interrupcion
	- Acceso de [[Dispositivo de  Entrada-Salida]]


# Componentes básicos del sistema

- CPU
	- ALU: realiza operaciones básicas
	- uc: unidad de control
	- Dos modulos (Registros)
		- MAR próxima dirección de memoria
		- MBR Contiene el dato a proceasr
- Memoria principal
- Dispositivos E-S (tienen sus propios MAR y MBR )
	- teclado
	- mouse
	- impresora...


## Ciclo de instruccion 

Son Busqueda y ejecucion

- **Comienzo** (Cargar en el contador de programa la dirección donde inicia el programa)
- **Busqueda** (ir a la posicion y buscar todos los datos que necesitamos)
- **Ejecucion** (Ejecuta la instruccion, y segun el resultado puede ir al acumulador o a la memoria o a la ALU o alterar la secuencia de ejecución)
- **Parar**

## Ciclo de Interrupción

Al recibir una instrucción la CPU
- Guarda el Contador de Programa  (CP), datos y dirección de lo que estaba haciendo
- Carga en el CP instrucciones de inicio del programar de interrupción


## E/S -> CPU


## E/S -> Memoria
liberar a la CPU del proceso (DMA)

# Estructuras de interconexion

## [[Bus]]
-  Conectan 2 o más dispositivos
- Son compartidos

Bus de 8 bytes, lleva 8 cables
sistema de 64 bist... maneja 64 bits a la vez

### Tipos de bus
LOs buses son el embudo en la velocidad de los pc
La memoria principal está muy pegada a la CPU para que los datos lleguen más rápido

**Bus de Datos**: Es el camino que se usa para  transferir entre módulos

**Bus de Dirección**: camino desde donde seleccionamos una dirección de memoria o un dispositivo E/S, el dato que saque se va a través del bus de datos

**Bus de Control**: Gobierna el uso y acceso a datos y direcciones 

### Lineas de Buses
- Dedicadas: Solo una función
- No dedicadas: Compartidas, varios elementos requieren sistema de arbitraje

### Sistema de arbitraje: 
determina las prioridades del uso bus, se peude aumentar el nivel de prioridad

- **Centralizados**: 
	- El arbitro no sabe cuantos dispositivos hay
	- Solo puede saber si hay o no solicitudes
	- PRIORIDAD MÁS CERCANA AL ARBITRO
- **Distribuidos**
	- Igual, solo que no hay arbitro



# Temporización

- Los sistemas funcionan de una manera _Sincrona_ o _Asincrona_
- Los + usados son forma asíncrona
- Oscilador (Reloj) , que oscila una frecuencia exacta F= 100MHz
- El ciclo es el periodo
- El periodo o ciclo es el inverso de la frecuencia 


## Puertas triestado

- Es un interruptor
- Indica que el driver está desconectado electricamente
-  NO hay ni 0 ni 1, el cable está desconectado electricamente