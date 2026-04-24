# grupo-01

## integrantes

- Bruno Ferrari // chknngttts
- Martina Echavarría // martinaechavarria-stack
- Lucas Ortiz // ryukivol

## descripción del sintetizador realizado

Al hablar como grupo sobre lo que queríamos hacer, pensamos en distintos synths y nos interesó mucho hacer uno que lograra producír sonidos más parecidos al noise (como genero musical). Al buscar "Pink/Brown/Blue/Drone noise generator" en internet, encontramos uno en un forum de electronica y circuitos llamado "https://electro-music.com". El circuito utilizaba componentes que ya aprendímos en clase pero permitía hacer nuevos sonidos. 

El "NANDulator - PHOBoS" utiliza un 4093* para generar el sonido. Dentro del esquematico en la pagina no muestran como amplificar la señal para que se pueda escuchar, por lo que decidimos añadir un LM386, conectando el pin 4 del 4093 al pin 3 del LM386. Eso si al utilizar el synth, sentimos que faltaba algo para poder modular más el sonido, por lo que añadimos un filtro de "https://generalguitargadgets.com" entre la salida del 4093 y el AMP. Consiste en 2 filtros R/C y un linear pot (todo conectado a un potenciómetro) que permite controlar el Dry/Wet del filtro, actuando como un EQ. 

En cuanto a modificaciónes de los circuitos base, en el Schmitt Trigger del pin 4-5-6 cambiamos el potenciómetro de 500k a 100k **CORROBORAR!!! CREO QUE ESTOY MINTIENDO**. En el filtro, cambiamos la resistencia de 39k por una de 36k (o 33k)**CORROBORAR!!! CREO QUE ESTOY MINTIENDO**, más que nada por la accesibilidad a materiales en el laboratorio y porque la variación de la resistencia es muy baja y no impacta el sonido final. 

*4093
  - El creador del NANDulator actualizó en su forum que distintos 4093 creaban resultados variados. Dependiendo de la empresa del chip, el circuito podía o no funcionar a corde a lo que tenia pensado el creador. Uno de los IC's que no funcionaba supuestamente es el CD4093 de Texas Instruments, que es el que utilizamos para el synth. De igual manera estamos contentos con el resultado, nos interesaría averiguar las variabilidades en sonido intercambiando el chip con otros de distintas empresas.

imagen del sintetizador en su contexto

![Esquemático Original del NANDulator](./imagenes/nandulatorplanosoriginales.gif)

audio o video del sintetizador en acción

![]()

![]()


## Componentes

En este proyecto utilizamos diferentes componentes cada uno para funciones especificas los cuales son:
- Resistencias: Se encargan de limitar el flujo de corriente eléctrica y establecer niveles de voltaje específicos dentro del circuito, las resistencias son fundamentales para proteger otros componentes más sensibles como los leds.
- Diodos: Actúan como ¨válvulas¨ que permiten el paso de la corriente en una sola dirección. Se utilizan generalmente para proteger el circuito contra inversiones de polaridad o para rectificar señales.
- Condensadores: Se encargan de almacenar energia temporalmente. 
- Potenciometros: Son resistencias variables que permiten ajustar manualmente el nivel de resistencia. Se utilizan para controlar diferentes parámetros como el volumen del audio o la intensidad de la señal.
- parlante: Es el ¨traductor¨ de salida que convierte las señales eléctricas amplificadas en ondas sonoras

Ademas diferentes chips, siendo estos:
- LMD386: Es un amplificador de potencia de audio de bajo voltaje. Su función principal es tomar una señal de audio débil y aumentarle la potencia lo suficiente para que pueda ser reproducida por el parlante con claridad.
  
- CD4093BE: Es un circuito integrado que contiene cuatro puertas NAND Schmitt Trigger, se suele utilizar para generar oscilacione, crear pulsos de reloj o limpiar señales con ruido gracias a su histéresis.

¿Que Son las compuertas NAND Schmitt Trigger y la histéresis?

- Las compuertas NAND son puertas lógicas que entrega una señal 0 solo cuando todas sus entradas están en 1, Si alguna entrada es 0, la salida será de 1. por otro lado el Schmitt Trigger es un diseño de circuito interno que le da "decisión" a la compuerta. En vez de tener un solo punto de cambio, tiene dos umbrales de voltaje distintos.

- La histéresis es la diferencia entre los dos umbrales del Schmitt Trigger, genra una sona de memoria de los V que se necesitan para apagar y encender un circuito, entregando una señal limpia a posibles interferencias 
## Proceso y resultados del reloj y secuenciador

con chips 555 y 4017

incluir texto e imágenes sobre cableado, pruebas, resultados obtenidos.
![]()
![]()


## Proceso y resultados de osciladores y amplificador

con chips 4093 y 386

incluir texto e imágenes sobre cableado, pruebas, resultados obtenidos.
![]()
![]()

4steps synth

+ Nuestro desarrollo: 

Desde el día martes 14 de abril, sesión 6a, desarrollamos el circuito en grupo durante las clases. Reiteradas veces rehicimos y analizamos el circuito pero no logró sonar del modo que debía, este no producía ningún sonido.

En el primer intento la secuencia de luces leds se terminaba la secuencia de prendido y apagado con un reatraso. Para aclarar el circuito de los leds debían  de ser un apagado y encendido espontaneo, lo cuál no nos resultó en nuestro primer intento de desarrollo en la protoboard. Luego pudimos encontrar nuestro error en la protoboard, lo resolvimos y  funcionó con la secuencia y frecuencia adecuada.

Al momento de conectar el clock generator y el sintetizador notábamos que todo iba con los resultado esperados, las luces led se prendían y llegaba el voltaje por todo el conjunto de circuitos. Pero conectando el parlante y esperando a que se produjera el sonido, no sonaba nada más que un leve "cck" por menos de un segundo.

Reordenamos todos los cables por color, cambiamos los chips usados nes555, 4017 y 4093B e incluso cambiamos componentes básicos como la batería debido a una posibilidad de carga baja resultando en un bajo voltaje no suficiente para funcionar y hacer ruido.

Rehicimos y probamos de todo con el circuito en la protoboard pero nunca nos resultó.


## Modificaciones realizadas a los circuitos originales

incluir texto, imágenes sobre modificaciones realizadas a los circuitos originales, incluyendo el proceso de diseño, pruebas y resultados obtenidos.

incluir modificaciones en posición, chips, parámetros, valores, etc.
![]()
![]()


## Carcasas de cartón

textos, imágenes

incluir origen de materiales, decisiones de posiciones de los componentes, decisiones estéticas, pruebas, resultados obtenidos.
**CARTON DE DESECHOS, CINTA GAFFER COMO FORMA DE ACERCARSE A LAS CARCASAS DE ALUMINIO EN LAS QUE SUELEN ESTAR LOS EFECTOS MODULARES Y PERILLAS A LO LOCO/PARLANTE COLGANDO PORQUE QUEREMOS SALIR UN POCO DE LO COMODO(?) O CONVENIENTE(???)**
![]()
![]()


## Interconexión entre módulos

textos, imágenes, diagramas de interconexión
![]()
![]()


## Resultados finales

texto

imagen
![]()
![]()

video / audio
![]()
![]()

## Aprendizajes y errores


En el proceso de intentar hacer ambos synths, nos encontramos con varios problemas.

En cuanto al 4stepsynth de misaaaaa, nunca logramos hacerlo funcionar correctamente. Las primeras veces nos encontramos en la misma situación que varios de nuestros compañeros, donde todo parecía estar bien conectado, pero claramente algo pasaba ya que el sonido no se manifestaba en el parlante. El 555 y 4017 no fueron problema para nosotros, ya que si funcionaban los 4 steps y el reset, el problema se encontraba en la conexión entre el 4017 y el LM386. Los profesores nos ayudaron viendo el synth buscando lo que podría ser el problema, Aaron nos sugirió usar cables acorde a los colores para que todo esté más ordenado y sea más facil de leer. Volvimos a hacer el synth con cables acorde a las conexiones pero nuevamente algo hicimos mal.

En la siguiente clase, misaaaaa trajo una versión actualizada del synth con mejoras/alteraciones que podrían ayudar a que nos funcionara. Al intentarlo nuevamente, omitimos las luces en el 4017 y cambiamos las resistencias de conexión al LM386 además de añadir condensadores de desacople en cada conexión a VCC. Nuevamente no encontramos la solución a nuestro problema. De igual manera teníamos pensado desde el principio hacer un synth que nos permita hacer ruido (Pink Noise).

En el "brumarcas-ulator" (NANDulator + Big Muff + alteraciones), inicialmente no tuvimos problemas graves. La primera vez que intentamos armar el **NANDulator**, solo teníamos una protoboard pequeña, por lo que se nos hizo imposible armarlo completamente y confundimos los diodos en el esquemático por LEDs. Al saber esto, compramos una protoboard de 830 puntos y sacamos diodos del LID. Con el synth en una protoboard grande, diodos y un LM386 con parlante conectado al NANDulator, conectamos una batería y efectivamente funcionaba. Algo que inicialmente ignoramos es que en uno de los schmitt trigger conectamos los diodos de manera incorrecta (positivo donde debería ser negativo), esto afectó el potenciómetro haciendo que al usarlo no afectará el sonido de grán manera, si cambiaba levemente la frecuencia, pero solo si el resto de los potenciómetros estaban al mínimo. Esto fue corregido en la segunda versión del "brumarcas-ulator". 

En cuanto al "Big Muff", el único problema que nos encontramos fue usar los valores correctos en las resistencias y potenciómetro. La primera vez que añadimos el filtro al NANDulator el efecto funcionaba más como volumen que como EQ (R/C) ya que el potenciómetro era de 10K (En vez de 100K como aparece en el esquemático) y la resistencia (R1) era de 30k (En vez de 39k) Esto lo arreglamos cambiando el potenciómetro por uno de 1M y la R1 por una de 47K. Al hacer estos cambios el filtro suena más como un muffler.

Hicimos funcionar el filtro, pero no sabíamos qué estaba haciendo para que el sonido se atenuará. Buscamos videos explicando esto y logramos entender un poco más. Los filtros en general suelen estar compuestos con resistencias y condensadores y dependiendo del valor en ambos, ciertas frecuencias se ven afectadas. Esto sirve para bajar/aumentar frecuencias altas/bajas.

Un error final que nos afectó en la segunda versión del "brumarcas-ulator" fue al momento de soldar los potenciómetros con cables. La primera vez soldamos cables comunes (No dupont) a los potenciómetros, esto hacía difícil la conexión a la protoboard y los cables se desconectaban con el más mínimo movimiento. Entonces soldamos finales de cables dupont out a los cables ya soldados en los potenciómetros. Este fue un grave error ya que al conectar todo de vuelta nada sonaba. Sacamos los finales dupont y probamos nuevamente pero seguía sin sonar. Claramente pasó algo al soldar y mover la protoboard que contenía el 4093. 

No logramos identificar el problema exacto en esa versión por lo que hicimos una nueva de cero en una nueva protoboard. Esta segunda versión contiene todos los arreglos mencionados anteriormente y efectivamente suena como se suponía.

Más en general, a lo largo de todo el proceso siempre ocurrían los mismos errores que suelen ser simples como:
- Batería con poca carga
- Componente quemado
- Componente equivocado
- Componentes tocandose cuando no deberían
- Batería mal conectada
- No conectando ambas tierras/positivos en distintas protoboard
- Componentes con polaridad conectados al revez
- Cables mal organizados
- Cables mal conectados
  - Sobretodo en potenciómetros con cables/componentes conectados 1 pin hacia al lado

**NO LOGRAMOS HACER FUNCIONAR EL 4STEPSYNTH COMPLETAMENTE, PERO SI LOGRAMOS EL NANDULATOR, COSTO UNIR EL FILTRO/EFECTO DEL 4093 Y AL AMP, NOS COSTO ENTENDER COMO FUNCIONABA EL FILTRO, LA UNION DE CABLES ETC...**
![]()
![]()

## Conclusiones

sobre modularidad, materialidad, trabajo en equipo, trabajo electrónico, trabajo maquinal.
![]()
![]()

