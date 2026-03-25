# sesion-03a
## Apuntes clase Martes 24 de Marzo

---

### <ins>Referentes vistos en clase</ins>

#### **Gordon Matta-Clark**
* Artista estadounidense con descendencia chilena, se le conoce mayormente por sus obras de arte arquitectónicas en donde destripaba edificios y, por así decirlo, borraba partes de estas edificaciones de manera controlada. Sus padres fueron artistas (su padre, Roberto Matta, fue de descendencia chilena).
* Recientemente se está haciendo una obra basada en él y en sus obras, llamada Splitting/Absence.
#### **Club sonoro deportivo**
* Mezcla la natación con la electronica
*Usan micrófonos especializados para detectar cañerías averiadas, por lo que son eficaces bajo el agua y permiten escuchar el nado de las personas
*La obra contará con nadadores que harán distintas actividades
* La mayoría de equipos geófonos permiten seleccionar rangos de frecuencia para aislar el ruido de la fuga frente al ruido ambiental
#### **John Cage**
* Pionero en la musica electronica
* Usaba sonidos no cotidianos y ambientales
* Usaba cintas magnéticas y radios
#### **Merce Cunningham**
* Fue un bailarin estadounnidense.
* Fue pareja de Jhon cage.
* Era controvertido por hacer tiempos cortos de obras y también por no guiarse por la música, sino que John Cage y él componían para ellos mismos y la obra se basaba en eso.
* Realizó una pieza llamada “silenciosa” “4’33” en la cual el público realizaba los sonidos de las obras y no los músicos.
#### **David Tudor**
* Compositor de música experimental
* Pianista interesado por la electronica
* Paso del piano a la electronia
* Crea sus propios circuitos y dispositivos electrónicos para hacer música.
* No usaba sintetizadores comerciales

---

### <ins>Significado de palabras o para qué sirven ciertas cosas vistas en clase o que no recordaba⁣/ins>
* **C** = capacitor
* **Astable** = Inestable
* **Frecuencia** = Rapidez y repetición de este fenómeno.
* **Frecuencia** de oscilación, ejemplo de la fórmula usada para calcular el tiempo en un IC: f = 1.44 / ((Ra + 2 * Rb) * C)
* **Oscilación** = Movimiento repetitivo de ida y vuelta alrededor de un punto de equilibrio.
* **Parlante** = Es un imán que recibe la electricidad, funciona al recibir corriente, moviendo una bobina y un imán para vibrar un cono o diafragma y esto produce un sonido audible, una transducción.
* **Transducción** = Conversión de una seña, estímulo o energía de una forma a otra.
* **Capacitores** = Genera que no sea tan agresiva la oscilación, atenúa la señal, detecta diferencias (funciona como un trigger del TouchDesigner).
* **Capacitor 100 uF** = Suaviza o atenua más que uno de 10 uF.
* **Interruptores** = Hay 3 interruptores, como los de la luz de un cuarto, pushbutton son solo los que mantienen su estado de prendido solo en el tiempo que se tiene presionado, y botón latch espera cierto tiempo después de activarlo en desactivarse, como un botón de ascensor.

---

### <ins>Experimentación con el protoboard</ins>

#### **Uso de parlante**
* Se usaron unos cables pinza para conectar el parlante al protoboard, para esto se necesita conectar 2 cables pinzas, uno al negativo y otro al positivo. Para conectarlo al protoboard, se necesitó que el cable pinza mordiera un cable y el cable conectarlo a la proto.
* Produce un sonido oscilatorio igual al parpadeo de la luz LED, al momento de usar un potenciómetro, llega un punto en donde emite sonido sin oscilación audible y es constante.
* Se puede usar directo a la batería, pero no es recomendable, ya que consume muchos voltios
* Se puede usar la vibración del parlante para generar un ritmo generado por las vibraciones, haciendo que un cable quede suspendido en la bocina y, mientras rebota, se sostenga uno para que lo roce y genere vibración en el parlante
* Si se conecta negativo con negativo y positivo con positivo, la bocina se irá hacia delante
* Caso contrario, se irá hacia atrás.
* Dependiendo del capacitor, el sonido es más agudo, mientras más bajo el número de uF, pareciese más agudo.

#### **Uso de boton**
* Se reemplaza la corriente inicial y se usa un botón para intercambiar entre apagado y prendido.
* Tiene 4 patas: 2 negativas y 2 positivas.
* Una parte del botón es plana y así se identifica cómo posicionarlo para el protoboard.

---

### <ins>Encargos</ins>

#### **Documental “Variaciones Espectrales” sobre José Vicente Asuar**
Es un documental basado en José Vicente Asuar. Fue un ingeniero y músico, el cual realizó estudios en Alemania y en Chile. Se le conoce principalmente por ser el pionero de la música electrónica debido a que fundó el primer laboratorio enfocado en eso, esto fue construido en la Universidad Católica de Chile. Ahí compuso su primera pieza llamada “Variaciones espectrales”, la cual se considera una de las primeras piezas electrónicas del país. También fue premiado en diferentes premios en concursos internacionales de composición electroacústica.

Debido a los ritmos de la música electrónica, la danza se vio influenciada y atraída hacia este género, alcanzando cierta popularidad.
Pese a todo lo contado, se considera que quedó parcialmente olvidado por la historia de Chile (en un punto del documental casi no encuentran nada de él ni dónde está su paradero), por lo que se invita al redescubrimiento de Asuar y cómo fue su aporte a la historia sonora chilena y latinoamericana.

Asuar fue todo un referente para todo tipo de personas creativas que fueron inspirándose en él y en sus piezas y hazañas. Una de ellas fue crear un computador llamado **COMDASUAR**, del cual sus siglas vienen de **Computador Musical Digital-Analógico Asuar**. Su función era componer música mediante programación, en otras palabras, generaba sonido mediante cálculos numéricos. Este fue uno de los primeros computadores especializados en crear música en Latinoamérica, incluso antes de que los sintetizadores fueran algo común.

Debido al golpe de Estado en Chile, el desarrollo tecnológico y artístico sufrió una interrupción abrupta. En el documental, explica que con ello vino el neoliberalismo y con ello la música como comercio, a lo cual están en desacuerdo debido a que no consideran la música como algo comercial ni puede ser considerado de esa forma.
Luego de crear el computador, trabaja con un Atari y, controlando sintetizadores comerciales, compone unas obras y las combina con piezas de su computador, pero lamentablemente esto es aislado y no público.

En mi opinión, me parece algo importante que se conserve la memoria de José Vicente Asuar, debido a que su aporte en Chile fue un antes y un después en toda Latinoamérica y en el mundo. Muchas veces se le atribuye este tipo de innovaciones a Europa o a Estados Unidos, cuando en realidad este documental rompe totalmente esta idea, haciendo ver que su legado no es solo una inspiración para los próximos músicos, sino también una forma de resistencia al olvido que viven algunos de la historia chilena y que fueron de vital importancia.
 
#### **Expandir circuito entregado basado en el 555**

