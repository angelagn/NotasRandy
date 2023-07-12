Estudio Autodidacta [https://developer.android.com/guide?hl=es-419](https://developer.android.com/guide?hl=es-419)


Es un [[IDE]]  programas para teléfonos, relojes inteligentes, coches, robots
Es el programa oficial para desarrollar en android, tiene opciones para móvil, smartwach, tv, carros
[[GitHub]]

>- En el mundo de los móviles la actividad son las pantallas
>- El sdk es para que dispositivo se va a hacer la aplicación
>- Siempre se programa sobre una #API
>- minimum #SDK es para seleccionar la versión de android para la cual hacer la App, hay que averiguar cual es el android más utilizado en el mercado y así se decide para que android hacer la app
>- También hay que mirar mi versión de android, para hacer las pruebas en mi dispositivo móvil
>- Programar en [[Java]] o en [[Kotlin]]
>- 


## Extensión .xml

## Estructura del proyecto

- Manifest: permisos de Internet y otros permisos de la app
- Java: contiene el nombre de mi proyecto y  main activity, 
- en res (recursos) viene:
	- Drawdable: donde se guardan las imagenes
	- layout: para diseñar con el mouse (aqui trabajan los diseñadores)
	- mitmap: iconos
- Gradle Scripts: Los scripts de java 

Si hay problema con el #SDK [[SDK]]

[https://www.solvetic.com/tutoriales/article/8865-instalar-android-sdk-manager-ubuntu-20-04/](https://www.solvetic.com/tutoriales/article/8865-instalar-android-sdk-manager-ubuntu-20-04/)





## Tools 
sdk manager : para descargar otras versiones
Device manager:

## Otras opciones
Genymotion: es una compañía que hace lo mismo que android estudio, se descarga y  crea la maquina virtual para desarrollar apps para dispositivos android


https://www.genymotion.com/

Kid de dllo  = SDK
Entorno de Dllo  = IDE

[[Dispositivos móviles]]

# Android
cada version de Android proporciona un nuvo nivel de la API
Arquitectura de capas
	hardware proveedores
	Sistema opedrativo google
	Apps desarrolladores


El sistema operativo se basa en el núcleo de Linux (Kernel) y sobre este Android proporciona un entorno de ejecución. Además de programación en Java también se pueden introducir fragmentos de programa en C y C++. En la plataforma de desarrollo encontramos el kit Android Studio (SDK) y el entorno de desarrollo denominado ID.

## Recursos para el dllo

- Android Studio
	- SDK (cod fuente, emuladores...)
		- SDK Manager: herramient apara intalar componentes
		- Componentes: conjunto de librerias de cierta versión
		- Incorpora herramientas necesarias para el uso de emuladores
		- Los emuladores es lo que llamamos dispositivos virtuales Android o AVD. Un AVD se define a partir de un dispositivo real. (se puede modificar el hardware en el emulador, quitar camara etc)
		-  También si existen librerías adicionales instaladas, por ejemplo las necesarias para acceder a Google Play.
		- Android SDK viene con un emulador en el que podemos probar la mayoría de nuestras aplicaciones. Podemos simular GPS, llamadas entrantes, salientes, SMS, entradas por la pantalla y el teclado, reproducción de audio y vídeo, y comunicaciones por red. Todos los tipos de aplicaciones están soportadas: widgets, servicios y actividades. Se pueden instalar y desinstalar como si de un móvil real se tratara.
	- IDE
		-  Proporciona difenetes funcionalidades para crear las apps
		- es un editor de código especializado para Android, un editor visual para las interfaces gráficas de usuario. En este editor visual podemos diseñar las interfaces gráficas sin más que arrastrar componentes visuales sobre un lienzo de dibujo.
	- No incorpora el kit nativo de dllo NDK (xa trabajar con fragmentos de cod en C Y C++) Se instala por separado
	