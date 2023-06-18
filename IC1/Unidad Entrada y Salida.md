E/S proporciona un método de comunicación entre el sistema central y el usuario
Los periféricos no van conectados directamente porque los formatos de datos son diferentes  a los de la CPU, la velocidad de los periféricos es más lenta
[[Arquitectura Von Newman]] 

## Funciones E/S
- Comunicarse con CPU y memoria a través de los [[Bus]]es
- Comunicarse con los periféricos

## Técnicas de interacción de E/S con el sistema
- E/S controlada por programa
- E/S controlada por IRQs
- Acceso directo a memoria (DMA) _Direct Memory Access_ (Dispositivo capaz de transferir datos entre la Mp y el dispositivo de E/S)

# Unidad E/S
1. Dispositivos externos (periféricos)
	- Categorías:
		- Adaptados al usuario
		- Adaptados a la máquina
		- De comunicación
		- De interacción con el medio externo
2. Controlador E/S
	-  Funciones:
		- Control y temporización
		- Comunicación con la CPU
		- Comunicación con el dispositivo externo
		- Almacén temporal de datos
		- Detección de errores
	- Requerimientos de comunicación con la CPU
		- Decodificación de la orden
		- Datos
		- Información sobre el estado
		- Reconocimiento de la información
			![[EstructuraDelControladorEntradaSalida.png]]
		- Estructura del sistema E/S
			- Métodos de interconexion E/S <==> CPU
				- E/S aisladas
					- Buses independientes
					- Bus común pero lineas de control separdas
				- E/S localizada en memoria
					- Bus único
3. E/S controlada por programa (La CPU está  pendiente del estado de la E/S ejecutando un programa de sondeo)
	- Ordenes de E/S
		- De control (Decirle que hacer)
		- De comprobación (Ver su estado)
		- De lectura
		- De escritura
	- Instrucciones de E/S
		- Localizada en memoria (mismas instrucciones que las de acceso a memoria)
			![[InstruccionesESEnMemoria.png]]
		- Aislada (Instrucciones especificas ==IN - OUT==)
			![[InstruccionesESAislada.png]]
1. E/S controlada por interrupciones
2. Acceso directo a memoria
3. Procesador E/S

# Canal multiplexor
La velocidad máxima para la E/S es la suma de las velocidades de cada dispositivo conectado