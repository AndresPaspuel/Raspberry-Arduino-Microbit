
1.- Planteamiento del Problema  
Para arquitectura de computadoras es primordial conocer todos los componentes de las tarjetas de Rapsberry pi, Arduino Uno y Microbit necesitamos adquirir conocimiento de cómo están conformadas estas tarjetas desde sus partes su funcionamiento, y como se programa en estas tarjetas por eso partimos de analizar el hardware, software y plantear dos ejemplos de cada tarjeta.
2.- Objetivos 

Objetivo General
Analizar el funcionamiento independientemente de cada tarjeta y conocer las partes que conforman cada tarjeta como ponerlas a funcionar y aplicar en ejemplos practicos.
Objetivos Específicos
•	Investigar a fondo las partes que conforman cada tarjeta desde su composición y su funcionamiento.
•	Ampliar los conocimientos y analizar la parte de software que necesita cada tarjeta para su funcionamiento.
•	Implementar todo lo adquirido en ejemplos prácticos y dinámicos. 


3.- Estado del Arte 
En el año 2012, como parte de un programa llamado Proyecto de conomiento en informática de la BBC se planeó un dispositivo para la enseñanza llamada BBC MicroBit que fue diseñada para animar a los niños a programar y consruir nuevas cosas, de modo que no fueran simples consumidores de dispositivos a lo largo del tiempo se fueron incorporando más potenia informática y nuevos sensores 
En el año 2017, en el Reino Unido, estas personas Sentance, S., Waite, J., Yeomans, L. y MacLeod, E iniciaron con un estudio, respecto a la computación informática que no es nada más que observar cual es el resultado de la utilización del micro bit tanto en estudiantes como profesores, y que lograron concluir que a practicas genera un compromiso para seguir creando e innovando en la mentalidad de cada persona.
En el año 2018 en España de llevo una investigación que estaba a cargo Carmen López de la Torre y que planteaba la posibilidad d trabajar con la tecnología microbit para la programación y que había logrado concluir que la práctica es fundamental debido a que no solo con teoría se aprende y que hay que aprovechar porque desarrolla la programación.
 En el año 2013 en Malacia se llevó un proyecto que se trataba de una alarma con incendios con sistema de monitoreo en tiempo real que detecta la presencia de humo en el aire debido al fuego y captura imágenes a través de una cámara instalada dentro de una habitación cuando ocurre un incendio. Los sistemas integrados utilizados para desarrollar este sistema de alarma contra incendios son Raspberry Pi y Arduino Uno. La clave fundamental de este proyecto fue que cuando se detectaba el humo el sistema mostrara una imagen del estado de la habitación desde una página web con esto se llevaría a cabo un gran avance debido que junto a la programación y esta tarjeta se puede evitar avisos falsos, llamadas telefónicos de personas maliciosas que lo que buscan es alterar la paz de la comunidad 
4.- Marco Teórico  
Hardware
Raspberry Pi

El Raspberry Pi es una plataforma de desarrollo de múltiples aplicaciones cuyo principal objetivo es propulsar la iniciativa de inventar, crear e innovar. Es una gran opción debido a que su precio no es elevado y nos ofrece una gran variedad de características a continuación veremos el detalle técnico desde el primer micro-procesador hasta el actual que es el Raspberry pi 4 Modelo B en donde vamos a notar claramente su evolución durante el tiempo.
Notaremos en la Raspberry Pi 4 Modelo B que se han incluido muchas más funcionalidades con el fin de que siga siendo de alto rendimiento y entre los muchos cambios que se observan en la Raspberry Pi 4 Modelo B es de un actualización a un procesador principal de próxima generación, una conectividad mejorada en Bluetooth, de igual manera se ha visto como ha mejorado la administración de energía, con una fuente de alimentación actualizada desde 2.5 amperios  y para admitir dispositivos USB externos más potentes.
Los cuatro puertos USB integrados de la Raspberry Pi 4 Modelo B proporciona suficiente conectividad como para un mouse, teclado o cualquier otro producto que se pueda llegar a necesitar también se puede agregar un concentrador USB pero se recomienda que este tenga su fuente de alimentación propia para no sobrecargar el regulador de voltaje de la tarjeta, no cuenta con botón de encendido y por ese motivo la tarjeta comenzara arrancar apenas tenga una alimentación de energía y para apagarlo solo se tendrá que desconectar la energía
Descripción de hardware
	Procesador de aplicaciones nRF51
Es donde se ejecutan los programas de usuario. Una sola aplicación completa que incluye código de usuario, código de tiempo de ejecución y pila de bluetooth se carga y ejecuta directamente desde la memoria flash del chip. 
	Comunicación inalámbrica Bluetooth
El transceptor integrado de 2.4GHz admite comunicaciones Bluetooth a través del Nordic S110 SoftDevice, que proporciona una pila Bluetooth de baja energía totalmente calificada. 
	Comunicaciones de radio de bajo nivel
El transceptor a bordo de 2.4GHz admite otros estándares de comunicaciones de radio, incluido el protocolo patentado Nordic Gazell. 
Nordic Gazell: proporciona una interfaz de radio de transmisión de paquetes pequeños muy simple entre otros dispositivos que admiten este protocolo propietario, como otros dispositivos micro: bit.  
	Botones
Botones en la parte frontal del micro: bit (2), y el botón 1 en la parte posterior, se presionan momentáneamente para hacer botones. El botón de retroceso está conectado al procesador de interfaz KL26 y al procesador nRF51 para restablecer el sistema. Esto significa que la aplicación se reiniciará independientemente de si está alimentada por USB o por batería. Los botones frontales A y B se pueden programar en la aplicación del usuario para cualquier propósito. Los botones A y B están conectados a pines GPIO que también son accesibles en el conector micro: bit edge.
	Monitor
La pantalla es un conjunto de 5x5 de LED. El software de tiempo de ejecución actualiza repetidamente esta matriz a alta velocidad, de modo que esté dentro de la persistencia del usuario del rango de visión y no se detecte parpadeo.  
	Sensor de movimiento
La variante 1.5 micro: bit tiene:
•	Un chip combinado de acelerómetro y magnetómetro que proporciona detección de 3 ejes y detección de intensidad de campo magnético. 
•	También incluye algo de detección de gestos a bordo (como la detección de caídas) en hardware y detección de gestos adicional (por ejemplo, logotipo arriba, logotipo abajo, sacudida) a través de algoritmos de software. 
•	El v1.5 micro: bit tiene una huella para dos sensores de movimiento diferentes: uno fabricado por ST (el LSM303AGR) y otro por NXP (FXOS8700CQ). El micro: bit DAL es compatible con ambos sensores y los detecta en tiempo de ejecución. Hasta la fecha, todas las placas v1.5 se han fabricado con el LSM303AGR. Si tuviéramos que pasar a la parte de NXP, se requeriría una ronda de pruebas y notificaríamos a la lista de correo DAL y Dispositivos. 
	Sensor de temperatura
El procesador de aplicaciones nRF51 tiene un sensor de temperatura central incorporado. Esto se expone a través del software estándar de tiempo de ejecución y proporciona una estimación de la temperatura ambiente.
	Pines de entrada / salida de uso general
Los pines 0, 1 y 2 son flexibles y se puede utilizar como pines de propósito general de entrada y salida (GPIO).
	Fuente de alimentación
Se puede proporcionar a través de la conexión USB o a través de una batería conectada al conector superior. Rango de operación es de 1.8 V a 3.6 V.
	Interfaz
El chip de interfaz maneja la conexión USB y se utiliza para actualizar el nuevo código al micro: bit, enviando y recibiendo datos seriales de un lado a otro a su computadora principal.
	Comunicaciones USB
El micro: bit tiene una pila de comunicaciones USB integrada. Esta pila proporciona la capacidad de arrastrar y soltar archivos en la unidad MICROBIT para cargar código en el procesador de la aplicación. 
	Depuración
Se conecta al procesador de la aplicación a través de 4 cables de señal. El código del procesador de la interfaz KL26 también se puede depurar a través de su interfaz integral de depuración del software SWD, por ejemplo, para cargar el código inicial del cargador de arranque en este procesador en el momento de la fabricación, o para recuperar un cargador de arranque perdido.

Arduino Uno
 



1.	Conector USB, que puede ser tipo B o mini, este provee la comunicación para la programación y la toma de datos, también provee una fuente de 5VDC para alimentar al arduino, pero de baja corriente por lo que no sirve para alimentar motores grandes por ejemplo. Siempre que adquieran una placa de arduino no olviden pedir el cable de conexión USB pues este representa unos $7000 adicionales.
2.	Regulador de voltaje de 5V, se encarga de convertir el voltaje ingresado por el plug 3, en un voltaje de 5V regulado. necesario para el funcionamiento de la placa y para alimentar circuitos externos. 
3.	Plug de conexión para fuente de alimentación externa, el voltaje que se suministra por aquí debe ser directo  y estar entre 6V y 18V, incluso 20V,  generalmente se usa un adaptador, pero debe tener cuidado de que el terminal del centro del plug quede conectado a positivo ya que algunos adaptadores traen la opción de intercambiar la polaridad de los cables.
4.	Puerto de conexiones; constituido por 6 pines de conexión con las siguientes funciones: RESET, permite resetar el microcontrolador al enviarle un cero lógico. Pin 3.3V, este pin provee una fuente de 3.3VDC para conectar dispositivos externos como en la protoboard por ejemplo. Pin 5V, es una fuente de 5VDC para  conectar dispositivos externos. Dos pines GND, que proveen la salida de cero voltios para dispositivos externos. Pin Vin, este pin esta conectado con el positivo del plug 3 por lo que se usa para conectar la alimentación de la placa con una fuente externa de entre 6 y 12VDC en lugar del plug 3 o la alimentacion por el puerto USB. Este puerto esta modificado en la versión R3 de Arduino Uno.
5.	Puerto de entradas análogas, aquí se conectan las salidas de los sensores  análogos. Estos pines solo funcionan como entradas recibiendo voltajes entre cero y cinco voltios directos.
6.	Microcontrolador Atmega 328, es el microcontrolador implementado en los Arduino uno y sobre el cual vamos a programar, en la versión SMD del arduino uno R2, se usa el mismo microcontrolador pero en montaje superficial, en este caso las únicas ventajas que se me ocurren son la reducción del peso y ganar un poco de espacio.
7.	Botón de RESET, este botón asi como el pin mencionado anteriormente permiten resetear el microcontrolador haciendo que reinicie el programa. En la versión R3 este pulsador se ubica arriba del conector USB, esto es un acierto pues al colocarle las Shield encima del arduino, se perdía la opción de resetear dado que este pulsador quedaba tapado.  
8.	Pines de programación ICSP, son usados para programar microcontroladores en protoboard o sobre circuitos impresos sin tener que retirarlos de su sitio.
9.	LED ON, enciende cuando el Arduino esta encendido.
10.	LEDs de recepción y transmisión, estos se encienden cuando la tarjeta se comunica con el PC. El Tx indica transmisión de datos y el Rx recepción.
11.	Puerto de conexiones, esta constituido por los pines de entradas o salidas digitales desde la cero hasta la 7. La configuración como entrada o salida debe ser incluida en el programa. Cuando se usa la terminal serial es conveniente no utilizar los pines cero (Rx)  y uno (Tx). Los  pines 3, 5 y 6 estan precedidos por el símbolo ~ , lo que indica que permiten su uso como salidas controladas por ancho de pulso PWM.
12.	Puerto de conexiones, incluye 5 entradas o salidas adicionales (de la 8 a la 12), las salidas 9, 10 y 11 permiten control por ancho de pulso; la salida 13 es un poco diferente pues tiene conectada una resistencia en serie, lo que permite conectar un led directamente entre ella y tierra. Finalmente hay una salida a tierra GND y un pin AREF que permite ser empleado como referencia para las entradas análogas.
13.	Este led indica el estado del pin 13.
14.	No se exactamente la función de estos pines.
15.	Chip de comunicación que permite la conversión de serial a USB.
Software
BBC Micro:Bit (https://microbit.org/)
Micro:Bit es una pequeña es un dispositivo que incorpora una matriz 5x5 leds que pueden mostrar mensajes de una manera relativamente sencilla incorporado en ella botones programables que pueden utilizarse para interactuar con el microcontrolador y se puede programar con un lenguaje de bloques JavaScript al igual que con Java o con Micropyton, que es un lenguaje similar al de Python pero diseñado para funcionar en pequeños microcontroladores como BBC Micro:Bit dando la posibilidad de programar con una aplicación a través de los sistemas Android e iOS.
en este microprocesador se puede programar de diferentes formasy entre las tres opciones tenemos el editor de bloques JavaScript que es un lenguaje fácil de entender se puede elegir entre JavaScript de Code Kingdoms o el block editor de Microsoft donde podemos cargar funciones y variables y consiste principalmente en seleccionar casillas de un lenguaje de programación.
 
Otra opción es la de programar con MicroPython que es una pequeña variación de Phython así permitiendo programar de manera más sencilla ciertas cosas y este tipo de programa es muy popular debido a sus potentes funciones y su comprensión del código encontramos la versión para programar offline que nos sirve cuando no tengamos conexión y poder seguir trabajando en proyectos en el interfaz de esta página tenemos la barra de herramientas el primero que esta es download y nos va a servir para descargar archivos .hex una vez que terminemos de programar alado de ella está la opción de guardar y estará habilitada una vez que nos encontremos registrados de igual manera se pueden importar archivos programados con otro editor de Python. 
 
Tinkerdcad (arduino)
Es una colección que incluye herramientas de software de Autodesk que permite a los principiantes crear modelos 3D. Sin embargo, ofrece también la posibilidad de montar, programar y simular circuitos con Arduino debido a que su pagina es amigable con el usuario y debido a ello no mostraría dificultad al momento de iniciar con cualquier programa a trabajar.
 
 WITH CODE .UK (Raspberry Pi)

Create.withcode.uk
 Es una herramienta  o pagina gratis que le permite escribir, ejecutar, depurar y compartir programas de Python en su navegador web.No necesita descargar ni instalar nada. Los programas de Python no pueden acceder a sus archivos o dañar su computadora, por lo que es una forma segura de aprender a crear con código.
 Python es un lenguaje de programación interpretado cuya filosofía hace hincapié en la legibilidad de su código. Se trata de un lenguaje de programación multiparadigma, ya que soporta orientación a objetos, programación imperativa y, en menor medida, programación funcional. Es un lenguaje interpretado, dinámico y multiplataforma.

 

Ejercicios de MicroBit 
1)Crear un programa que mediante un aviso acústico se advierta de que la micro:BIT está recibiendo la temperatura del ambiente.
Utilizando MakeCode de https://makecode.microbit.org/#editor
 
Utilizando Phyton en https://makecode.microbit.org/#editor
 

2.Crear un juego en Microbit donde al pulsar el botón A y B, con los pines 0 y 1 realice movimientos de izquierda a derecha , de arriba hacia abajo para llegar al led con brillo sin llegar a tocarnos con una casilla que contenga una bomba al llegar al objetivo desplegara una carita feliz al contrario de estar en una casilla con una bomba saldrá una carita triste y un enunciado que diga Gameover. 
Utilizando MakeCode de https://makecode.microbit.org/#editor
 






Utilizando Phyton en https://makecode.microbit.org/#editor
 


Ejercicios de Arduino
Ejercicio 1
Realizar una secuencia de leds con Arduino
 

Ejercicios 2 
Se diseña un programa que se prende dos led conectados al arduino en los pines de entrada y salida, se prenderan y se apagaran cada 1000ms.

 





Ejercicios de Raspberry Pi
Ejercicio 1
Utilizando la página https://create.withcode.uk/ realizamos un ejercicio que nos va a pedir un número el cual significa la cantidad de veces que lo vamos a repetir luego de realizar el ingreso de números nos desplegara en pantalla cuantos números pares e impares ingresamos
 
Ejercicio 2
Digitar las tres notas para saber si el alumno aprueba o no.
 ![image](https://user-images.githubusercontent.com/63418581/85350544-009cf780-b4c7-11ea-89d2-68da133e3ab9.png)

 

