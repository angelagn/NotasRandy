[[Arquitectura Von Newman]] [[Unidad Entrada y Salida]]
Eliminar los bucles de espera
Cuando el periférico preparado para intercambiar información fuerza una interrupción en la tarea de la CPU para atender a la E/S una vez transferido, la CPU continúa la tarea.

==Línea de petición de interrupción (PI):== está entre la CPU y E/S

Cuando el periférico activa la petición de la interrupción la mantiene activada hasta que se atiende su petición

- La PI se mantiene activada durante la respuesta a la interrupción
- Durante la respuesta, la interrupción permanece inhabilitada

# Métodos
- La propia CPU ignora la PI cuando responde al programa con la primera instrucción
- El propio sistema tiene un mecanismo de enmascaramiento de interrupciones

# Tratamiento de una interrupción
1. Activar el sistema de interrupciones
2. Periférico activa PI
3. CPU termina instrucción en curso, salva el PC y otros registros usados por el programa
4. CPU inhibe interrupciones (más caras) u carga en el PC el vector interrupción (dirección de localización del programa de respuesta)
5. Se informa a periférico de fin de respuesta ( Línea RI) para que desactive PI
6. Se reactiva el sistema de interrupciones
7. Se recupera el PC y los registros => se continúa con la ejecución del programa

# Clasificación de las interrupciones IRQs
- Origen
	- Externa (periféticos)
	- Interna (La propia CPU)
- Número de líneas
	- 1 linea
	- Múltiples líneas
- Control de la CPU sobre la IRQ 
	- Enmascarables
	- No enmascarables
- Fuente de la interrupción (identificación)
	- Múltiples líneas
	- Encuesta
	- Vectorizadas
- Gestión de la prioridad
	- Por software
	- Por hardware
- Niveles de interrupción
	- Ünico
	- Multinivel

## Origen
- Externas
	- Generada por periférico
	- Fallo alimentación
	- Señal de reloj
	- Acceso a memoria **no permitido**
	- Sistemas multiprocesadores
- Internas
	- Desbordamiento de la ALU
	- Código de operación desconocido
	- Interrupción de rastreo
	- Interrupción de programa

## Número de líneas de interrupción
- Varias líneas
- Única línea para varios periféricos

## Control de la CPU sobre la interrupción
- Enmascaramiento individual
- Enmascaramiento por nivel

## Identificación de la fuente de IQR y gestión de la prioridad
- identificación mediante encuesta (única línea y cuando hay IQR se encuesta a los perifericos)
- mediante encadenamiento (encuesta pro hardware, interrupciones vectorizadas)
- Mediante hardware paralelo (Usa registro de interrupción, registro interrupción + registro máscara)




Volver a [[Unidad Entrada y Salida]]