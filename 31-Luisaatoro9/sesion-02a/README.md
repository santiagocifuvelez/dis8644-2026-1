# Sesión 02a: Martes 17 de marzo 
**Temas:** Lectura de esquemáticos, código de colores en resistencias y análisis de referentes (Kraftwerk / LCD Soundsystem).
## 1. Apuntes
kit: una batería Energizer de 9V, cables de cobre, una Protoboard (la placa de pruebas donde pinchamos todo) y un set de componentes que incluye resistencias de diversas capacidades, LEDs de colores y algunos chips (circuitos integrados como el NE555P).

Circuito eléctrico es gestionar un **lazo cerrado de energía**. 

Cómo leer un Esquemático (Mapa de Flujo) Un esquema técnico es una abstracción. Reglas críticas para no cometer errores de conexión: 
* **Nodos de Conexión:** Identificamos los puntos negros donde los cables se unen físicamente. Si las líneas se cruzan sin punto, no hay contacto eléctrico.

* **Diferencia de Potencial:** La energía fluye desde **VCC** (9V) hacia el retorno a tierra o **GND** (0V). Sin este camino cerrado, los electrones no circulan.
* **Sentido de Lectura:** se leen de izquierda a derecha (entrada a salida) y de arriba hacia abajo (potencial alto a tierra).
* **El Código de Colores:** Precisión en el Diseño Para identificar las resistencias (que miden la oposición al flujo en **Ohms $\Omega$**), aplicamos un sistema visual.
* **La Regla de la Tolerancia:** Buscamos la banda **Dorada** y la situamos a la **derecha**. Empezamos a leer desde el extremo opuesto.
* **El Multiplicador:** La tercera banda es clave. Por ejemplo, en una resistencia de **220 $\Omega$**, vemos **Rojo (2), Rojo (2) y Café (x10)**. Si esa tercera banda cambiara a Rojo, el valor subiría a 2.200 $\Omega$, alterando todo el comportamiento del circuito.

A diferencia de los LEDs o el Chip 555, las resistencias **no tienen polaridad** (dirección). Se pueden instalar en cualquier sentido, lo que facilita el ruteo(camino) en la protoboard.

🧮Ley de Ohm Ω

$V=I⋅R$

Donde V es el voltaje, I es la corriente y R es la resistencia medida en Ohms.

# 2. Referentes: Kraftwerk y LCD Soundsystem 
Para esta sesión, elegí dos discos que son clave para entender cómo la tecnología se vuelve música. 
Kraftwerk: *The Man-Machine* (1978) 
Este disco es que fue grabado en su propio estudio, el **Kling Klang**. En esa época no solo compraban sintetizadores, ¡ellos mismos diseñaban su hardware! 
* **Análisis:** Al escucharlo, siento que cada sonido es súper limpio y matemático. En temas como *"The Robots"*, la voz suena robótica porque usan un **Vocoder**, que básicamente convierte la voz en una señal eléctrica para controlar el sintetizador.
* **Contraste:** En los 70 se veían llenos de cables y perillas reales en el escenario; hoy usan proyecciones 3D. Ha cambiado la tecnología visual, pero esa "perfección mecánica" sigue ahí.
  
LCD Soundsystem: *Sound of Silver* (2007) Este disco es el polo opuesto. James Murphy se aisló en una granja y forró las ventanas con papel aluminio para no saber qué hora era mientras grababa. 
* **Lo que escucho:** A diferencia de Kraftwerk, aquí hay mucho "caos controlado". Mezclan baterías reales con sintetizadores analógicos. Me gusta mucho cómo usan el **ruido blanco** (ese sonido como de estática) para crear tensión.**En vivo:** Son un desorden de cables y potenciómetros. Se nota que hay un esfuerzo físico al tocar, muy parecido a lo que nos pasa a nosotros peleando con los cables en la protoboard.
  
En conclusión todo esto me hace pensar que la electrónica es, al final, una forma de **componer con energía**. Desde elegir una resistencia de 220 $\Omega$ para que no se queme un LED, hasta filtrar una frecuencia en un sintetizador, todo es diseño. Ya no veo los aparatos como "cajas negras", sino como sistemas que puedo entender y manipular.

* **Documental:** *The Internet's Own Boy* (2014) - Ref. Sesión anterior.
* **Teoría:** Manual de códigos de colores para resistencias de 1/4W.
* **Artículo:** [Kraftwerk and the electronic revolution](https://www.britannica.com/topic/Kraftwerk) - Encyclopedia Britannica

### Ejercicios
Me enfoque en ver qué pasaba con los LEDs al retirar diferentes resistencias del circuito. Aquí anoté lo que observé en cada ejercicio:

1. Al empezar con el primer circuito, me di cuenta de que la **R1** es clave: si la quitas, se apaga todo porque cortas el flujo principal. En cambio, si sacas la **R2** o la **R5**, solo se queda prendida la **D4**. Cuando probe quitando la **R3**, las tres primeras luces (**D1, D2, D3**) seguían funcionando sin problemas. 

2. Aquí el comportamiento cambió un poco. Por ejemplo, al retirar la **R1**, la **D2** se apagó de inmediato. Lo más curioso fue que al quitar la **R5**, la **D1** dejó de brillar por falta de flujo, pero las otras seguían bien. También note que quitar **R6** o **R7** no afectaba en nada al encendido de los LEDs; el circuito parecía ignorar ese cambio. 

3. En la última prueba, el circuito era más robusto. Si quitába **R1** o **R2**, no pasaba nada, todo seguía prendido, pero se ponía sensible con otras: si sacabas la **R4** o la **R5**, tanto la **D2** como la **D4** se apagaban al mismo tiempo. Al final, probe con la **R6** y solo se apagó la **D2**, dejando el resto del camino libre para la corriente.
