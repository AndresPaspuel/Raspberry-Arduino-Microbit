
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

-En el año 2012, como parte de un programa llamado Proyecto de conomiento en informática de la BBC se planeó un dispositivo para la enseñanza llamada BBC MicroBit que fue diseñada para animar a los niños a programar y consruir nuevas cosas, de modo que no fueran simples consumidores de dispositivos a lo largo del tiempo se fueron incorporando más potenia informática y nuevos sensores 

-En el año 2017, en el Reino Unido, estas personas Sentance, S., Waite, J., Yeomans, L. y MacLeod, E iniciaron con un estudio, respecto a la computación informática que no es nada más que observar cual es el resultado de la utilización del micro bit tanto en estudiantes como profesores, y que lograron concluir que a practicas genera un compromiso para seguir creando e innovando en la mentalidad de cada persona.
-En el año 2018 en España de llevo una investigación que estaba a cargo Carmen López de la Torre y que planteaba la posibilidad d trabajar con la tecnología microbit para la programación y que había logrado concluir que la práctica es fundamental debido a que no solo con teoría se aprende y que hay que aprovechar porque desarrolla la programación.
 
-En el año 2013 en Malacia se llevó un proyecto que se trataba de una alarma con incendios con sistema de monitoreo en tiempo real que detecta la presencia de humo en el aire debido al fuego y captura imágenes a través de una cámara instalada dentro de una habitación cuando ocurre un incendio. Los sistemas integrados utilizados para desarrollar este sistema de alarma contra incendios son Raspberry Pi y Arduino Uno. La clave fundamental de este proyecto fue que cuando se detectaba el humo el sistema mostrara una imagen del estado de la habitación desde una página web con esto se llevaría a cabo un gran avance debido que junto a la programación y esta tarjeta se puede evitar avisos falsos, llamadas telefónicos de personas maliciosas que lo que buscan es alterar la paz de la comunidad 


4.- Marco Teórico  

Hardware

Raspberry Pi

El Raspberry Pi

Es una plataforma de desarrollo de múltiples aplicaciones cuyo principal objetivo es propulsar la iniciativa de inventar, crear e innovar. Es una gran opción debido a que su precio no es elevado y nos ofrece una gran variedad de características a continuación veremos el detalle técnico desde el primer micro-procesador hasta el actual que es el Raspberry pi 4 Modelo B en donde vamos a notar claramente su evolución durante el tiempo.

Notaremos en la Raspberry Pi 4 Modelo B que se han incluido muchas más funcionalidades con el fin de que siga siendo de alto rendimiento y entre los muchos cambios que se observan en la Raspberry Pi 4 Modelo B es de un actualización a un procesador principal de próxima generación, una conectividad mejorada en Bluetooth, de igual manera se ha visto como ha mejorado la administración de energía, con una fuente de alimentación actualizada desde 2.5 amperios  y para admitir dispositivos USB externos más potentes.


Los cuatro puertos USB integrados de la Raspberry Pi 4 Modelo B proporciona suficiente conectividad como para un mouse, teclado o cualquier otro producto que se pueda llegar a necesitar también se puede agregar un concentrador USB pero se recomienda que este tenga su fuente de alimentación propia para no sobrecargar el regulador de voltaje de la tarjeta, no cuenta con botón de encendido y por ese motivo la tarjeta comenzara arrancar apenas tenga una alimentación de energía y para apagarlo solo se tendrá que desconectar la energía


MICRO BIT

![image](https://user-images.githubusercontent.com/63418581/85351996-97b77e80-b4ca-11ea-99c2-223b048fb641.png)


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

•	También incluye algo de detección de gestos a bordo (como la detección de caídas) en hardware y detección de gestos adicional (por 
ejemplo, logotipo arriba, logotipo abajo, sacudida) a través de algoritmos de software. 

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


![image](https://user-images.githubusercontent.com/63418581/85352089-c7ff1d00-b4ca-11ea-81ee-f01a8436afad.png)


Conector USB
Que puede ser tipo B o mini, este provee la comunicación para la programación y la toma de datos.
Regulador de voltaje de 5V
Es necesario para el funcionamiento de la placa y para alimentar circuitos  externos. 

Plug de conexión
Es para fuente de alimentación externa, el voltaje que se suministra por aquí debe ser directo  y estar entre 6V y 18V, incluso 20V
 

Puerto de conexiones; constituido por 6 pines de conexión con las siguientes funciones: RESET, Pin 3.3V, Pin 5V Dos pines GND, . Pin Vin.
 

Puerto de entradas análogas, aquí se conectan las salidas de los sensores  análogos.
Microcontrolador Atmega 328, es el microcontrolador implementado en los Arduino uno y sobre el cual vamos a programar.
 
Botón de RESET, este botón asi como el pin mencionado anteriormente permiten resetear el microcontrolador haciendo que reinicie el programa.
 
 
Pines de programación ICSP, son usados para programar microcontroladores en protoboard o sobre circuitos impresos sin tener que retirarlos de su sitio.
 
LED ON, enciende cuando el Arduino está encendido.
 
LEDs de recepción y transmisión, estos se encienden cuando la tarjeta se comunica con el PC.
 
 
Puerto de conexiones, está constituido por los pines de entradas o salidas digitales desde la cero hasta la 7

Puerto de conexiones, incluye 5 entradas o salidas adicionales

Este led indica el estado del pin 13.

No sé exactamente la función de estos pines.

Chip de comunicación que permite la conversión de serial a USB.
 


Software

BBC Micro:Bit (https://microbit.org/)
Micro:Bit es una pequeña es un dispositivo que incorpora una matriz 5x5 leds que pueden mostrar mensajes de una manera relativamente sencilla incorporado en ella botones programables que pueden utilizarse para interactuar con el microcontrolador y se puede programar con un lenguaje de bloques JavaScript al igual que con Java o con Micropyton, que es un lenguaje similar al de Python pero diseñado para funcionar en pequeños microcontroladores como BBC Micro:Bit dando la posibilidad de programar con una aplicación a través de los sistemas Android e iOS.

En este microprocesador se puede programar de diferentes formasy entre las tres opciones tenemos el editor de bloques JavaScript que es un lenguaje fácil de entender se puede elegir entre JavaScript de Code Kingdoms o el block editor de Microsoft donde podemos cargar funciones y variables y consiste principalmente en seleccionar casillas de un lenguaje de programación.
 
Otra opción es la de programar con MicroPython que es una pequeña variación de Phython así permitiendo programar de manera más sencilla ciertas cosas y este tipo de programa es muy popular debido a sus potentes funciones y su comprensión del código encontramos la versión para programar offline que nos sirve cuando no tengamos conexión y poder seguir trabajando en proyectos en el interfaz de esta página tenemos la barra de herramientas el primero que esta es download y nos va a servir para descargar archivos .hex una vez que terminemos de programar alado de ella está la opción de guardar y estará habilitada una vez que nos encontremos registrados de igual manera se pueden importar archivos programados con otro editor de Python. 


![image](https://user-images.githubusercontent.com/63418581/85351853-44453080-b4ca-11ea-98dd-60224ec3ade1.png)

Tinkerdcad (arduino)

Es una colección que incluye herramientas de software de Autodesk que permite a los principiantes crear modelos 3D. Sin embargo, ofrece también la posibilidad de montar, programar y simular circuitos con Arduino debido a que su pagina es amigable con el usuario y debido a ello no mostraría dificultad al momento de iniciar con cualquier programa a trabajar.

![image](https://user-images.githubusercontent.com/63418581/85351839-3db6b900-b4ca-11ea-82ed-04e261c42c2e.png)


 WITH CODE .UK (Raspberry Pi)

Create.withcode.uk
 Es una herramienta  o pagina gratis que le permite escribir, ejecutar, depurar y compartir programas de Python en su navegador web.No necesita descargar ni instalar nada. Los programas de Python no pueden acceder a sus archivos o dañar su computadora, por lo que es una forma segura de aprender a crear con código.
 
 Python es un lenguaje de programación interpretado cuya filosofía hace hincapié en la legibilidad de su código. Se trata de un lenguaje de programación multiparadigma, ya que soporta orientación a objetos, programación imperativa y, en menor medida, programación funcional. Es un lenguaje interpretado, dinámico y multiplataforma.

 ![image](https://user-images.githubusercontent.com/63418581/85351829-398a9b80-b4ca-11ea-9d3a-bb3a07225669.png)

Ejercicios de MicroBit 

1)Crear un programa que mediante un aviso acústico se advierta de que la micro:BIT está recibiendo la temperatura del ambiente.
Utilizando MakeCode de https://makecode.microbit.org/#editor

 ![image](https://user-images.githubusercontent.com/63418581/85351615-d3057d80-b4c9-11ea-984d-7de0d1c2bfbf.png)

Utilizando Phyton en https://makecode.microbit.org/#editor

![image](https://user-images.githubusercontent.com/63418581/85351597-cda83300-b4c9-11ea-9669-02f307e60916.png)
 

2.Crear un juego en Microbit donde al pulsar el botón A y B, con los pines 0 y 1 realice movimientos de izquierda a derecha , de arriba hacia abajo para llegar al led con brillo sin llegar a tocarnos con una casilla que contenga una bomba al llegar al objetivo desplegara una carita feliz al contrario de estar en una casilla con una bomba saldrá una carita triste y un enunciado que diga Gameover. 
Utilizando MakeCode de https://makecode.microbit.org/#editor


![image](https://user-images.githubusercontent.com/63418581/85351515-9174d280-b4c9-11ea-809a-3ddd4dfba36c.png)
 
Utilizando Phyton en https://makecode.microbit.org/#editor
![image](https://user-images.githubusercontent.com/63418581/85351443-5ffc0700-b4c9-11ea-8721-ae9b16c73109.png)


Ejercicios de Arduino

Ejercicio 1
Realizar una secuencia de leds con Arduino
 
![image](https://user-images.githubusercontent.com/63418581/85351127-95ecbb80-b4c8-11ea-8f3b-84e846f3edfe.png)

Ejercicios 2 
Se diseña un programa que se prende dos led conectados al arduino en los pines de entrada y salida, se prenderan y se apagaran cada 1000ms.


![image](https://user-images.githubusercontent.com/63418581/85350704-7739f500-b4c7-11ea-936c-6782b2f059f8.png)
 
Ejercicios de Raspberry Pi

Ejercicio 1

Utilizando la página https://create.withcode.uk/ realizamos un ejercicio que nos va a pedir un número el cual significa la cantidad de veces que lo vamos a repetir luego de realizar el ingreso de números nos desplegara en pantalla cuantos números pares e impares ingresamos

![image](https://user-images.githubusercontent.com/63418581/85350996-44dcc780-b4c8-11ea-9abf-530601dddf1b.png)
 
Ejercicio 2

Digitar las tres notas para saber si el alumno aprueba o no.

![image](https://user-images.githubusercontent.com/63418581/85350825-c5e78f00-b4c7-11ea-820f-c4b72867f1cd.png)
 

5.DIAGRAMAS 

ARDUINO UNO 

![image](https://user-images.githubusercontent.com/66221550/85352292-33e18580-b4cb-11ea-9582-45abaaa10463.png)
![image](https://user-images.githubusercontent.com/66221550/85352350-5b385280-b4cb-11ea-835e-f847349242a4.png)

6.- Lista de Componentes 

ARDUINO 

•	Arduino 

•	Leds (7) 

•	Resistencias de 320 ohmios

•	Código a utilizar

•	Leds (2)

•	Resistencias 320 ohmios 

MICRO BIT

•	Tarjeta Micro:Bit

•	sensor de temperatura(incluido en la tarjeta de Micro:Bit)

•	Salida de sonido

•	Pin 0 y 1

•	Bloques de Juego ,Entrada ,Variable,Funcion

RASPBERRY

•	Computadora para programar


7.- MAPAS DE VARIABLE

Raspberry

1.	print: Permite escribir caracteres del código ASCII.

2.	if , else: Son condicionales si existe más de una opción.

3.	int: Digitar datos enteros.

4.	input: Permite digitar datos de distintos tipos

5.	def: Permite crear objetos según lo defina el usuario.

6.	for: es un bucle que repite el bloque de instrucciones en un número predeterminado de veces.

7.	variables: Es un espacio reservado de la memoria que almacena un dato.

8.	Operadores Aritméticos: es la declaración de funciones matemáticas.

Arduino

1.	void setup, void loop: Sirve para ejecutar líneas de códigos. 

2.	pinMode: Configura cada pin de manera individual, agregando que sirve de entrada y salida

3.	delay: Permite que espere hasta su ejecución.

Arduino 

Microbit
1.	Establecer: Establece una variable para que sea igual a la entrada.

2.	Si, si no: es un condicional donde evaluará si es verdadero y ejecutara el primer bloque de declaraciones.

3.	Mostrar cadea: Muestra el texto en pantalla.

4.	Play melodía: toca una melodía del editor de melodías

Microbit ( Juego ) 
Micro Python

1.	def : Sirve  para crear objetos funciones definidas por el usuario

2.	Input : Datos que llegan al programa

3.	Globo : Es una variable accesible en todos los ámbitos 

4.	if : evalúa una condición

Bloques 

1.Bloques de Entrada

2.Bloques Variables (Jugador)

3.Bloque deFunciones

4.Bloque de Juegos

5.Bloque de Entrada

8. Explicación del código fuente

MicroBit

Ejercicio 1

Crear un programa que mediante un aviso acústico se advierta de que la micro:BIT está recibiendo la temperatura del ambiente. 

Usar el evento para siempre, para iniciar el programa.

Crear una variable donde se almacenará el valor del sensor obtenido por el bloque dirección de la brújula (º).

Se introduce el condicional si entonces si no para comprobar en qué intervalo se encuentra el valor obtenido por el sensor. Si el valor se encuentra entre 0º y 24º la micro:BIT es porque el sensor de temperatura marca un valor cálido caso contrario desplegará el mensaje “Frio” y seguidamente se reproducirá un sonido.

Ejercicio 2 

Crear juego en microbi donde al pulsar el botón A y B, con los pines 0 y 1 realice movimientos de izquierda a derecha  , de arriba hacia abajo para llegar al led con brillo sin llegar a tocarnos con una casilla que contenga una bomba al llegar al objetivo desplegará una carita feliz al contrario de estar en una casilla con una bomba saldrá una carita triste y un enunciado que diga Game Over. 

Raspberry Pi

Ejercicio 1. 

Ingresar por teclado n cantidad de números y cuántos números pares e impares existen
Para comenzar a programar en whithcode.uk deberemos tener bases de programación y para comenzar inicializamos dos variables en las que se van acumular nuestros valores.
Después de haber inicializado las variables preguntamos en pantalla cuantos numeros va a ingresar eso se guardará en nuestra variable num.

El siguiente paso sería implementar un bucle de repetición for en la que comenzaremos inicializando nuestra variable i y hasta donde queremos que llegue nuestro ciclo que en nuestro caso se repetirá el número de veces que se ha ingresado en num
Dentro de nuestro ciclo for comenzaremos a ingresar los números en nuestro arreglo.
Como siguiente paso tenemos que preguntar si el numero ingresado es par o no con una operación de sacar el residuo de un número y comparar si este es igual a 0 o no.

En el caso de que el número ingresado sea par se tomará como un contador y este almacenará el número de veces que paso x alli.

En el caso contrario almacenaremos el número de veces que fue un número impar 
Como último desplegamos en pantalla el número de veces que se han acumulado en nuestro contador.

Ejercicio 2.

Raspberry (Digitar las notas)

Lo que hace este programa es ver si el alumno pasa o no, entonces lo que hacemos es digitar las tres notas que correspondan ya una vez ingresado ls valores lo que hace es sumar la notas y en este punto vamos a utilizar los condicionales if y else porque si la suma de las tres notas da 42 o más despliega “pasa” pero si es menor a 42 despliega “no pasa”.

Arduino  

Ejercicio1


(Secuencia de leds)
en este ejercicio nosotros programamos la secuencia que deseamos y que leds van a prenderse según el tiempo que nosotros lo estipulamos, en este caso se lo programó con una duración de medio segundo y así seguirá hasta que complete la secuencia además de que este repite el ciclo.

Ejercicio2

(Encendido y Apagado de leds )
Se diseña un programa que se prende dos led conectados al arduino en los pines de entrada y salida, se prenderán y se apagaran cada 1000ms.

8.- Descripción de pre-requisitos y configuración 

1.	En el caso de arduino es necesario programar los terminales a utilizar en la secuencia de leds se utilizó terminales del 2 al 8 y las resistencias se las conecto a la GND para no generar un corto.
2.	Una buena conexión a internet ya que no se puede guardar el código mientras se este utilizando la versión de https://create.withcode.uk/ que sirve para crear funcionalidades e implementar en nuestra Raspberry Pi

9.- Aportaciones 

Una aportación clara que se puede ver es la de que tinkercad es una herramienta amigable y lo es más entendible para las personas que recién están empezando con simulaciones, a diferencia del proteus que en sí es una herramienta buena pero el único inconveniente es que no es amigable con el usuario debido a que todas sus funciones están escondidas y corresponde saber sobre su interfaz para encontrarla.

![image](https://user-images.githubusercontent.com/65547964/85354676-bcaef000-b4d0-11ea-8dea-0bdbd0aff5b2.png)
10.- Conclusiones 

 	El microprocesador Raspberry Pi es un dispositivo que posee muchas características positivas, pero así mismo es el más complicado de programar ya que tenemos que instalar el Sistema operativo.
  
 	Con los tres micro-procesadores es necesario tener un nivel medio en programación para poder realizar diseños y controles
  
 	El microprocesador Micro:Bit nos brinda una gran capacidad de interactuar y realizar de manera novedosa al momento de programar porque no exige un novel en programación. 
  
 	El microprocesador Arduino uno tiene bastantes beneficios no solo por su sencillez de encontrar sino también por su accesible plataforma y su sencilla programación que lo hace una herramienta ideal para jovenes aprendices , 

11.- Recomendaciones

 	Antes de empezar a utilizar cualquier simulador es adecuado el de tener una introducción hacia esa área porque si iniciamos sin conocer nada no podemos lograr el objetivo que tenemos en mente
  
 	Tener un cierto grado de conocimiento de programación porque en el lenguaje de Python puede llegar a confundir cuando técnicamente es lo mismo.

 	También es importante tener un conocimiento  adecuado de circuitos ya que estas tarjetas para hacerlas funcionar utilizamos diferentes herramientas como leds , resistencias  etc

12.- Cronograma
![image](https://user-images.githubusercontent.com/65547964/85354870-19aaa600-b4d1-11ea-94bc-3c674d10ac7b.png)

Bibliografía

Alegre, J. A. (2017). BBC Micro:Bit Introducción a la mecatrónica en estudios preuniversitarios. Valencia

Casco, S. M. (2014). Raspberry Pi, Arduino y Beaglebone Black Comparación y Aplicaciones. Universidad Catolica Nuestra Señora de la Asunción

Sentance, S., Waite, J., Yeomans, L. y MacLeod, E. (noviembre de 2017). Enseñanza con dispositivos informáticos físicos: la iniciativa BBC micro: bit. En Actas del 12º Taller sobre Educación Informática Primaria y Secundaria (pp. 87-96).

MS Bin Bahrudin, RA Kassim y N. Buniyamin, "Desarrollo del sistema de alarma contra incendios utilizando Raspberry Pi y Arduino Uno", Conferencia Internacional 2013 sobre Ingeniería Eléctrica, Electrónica y de Sistemas (ICEESE) , Kuala Lumpur, 2013, pp. 43-48, doi: 10.1109 / ICEESE.2013.6895040.



