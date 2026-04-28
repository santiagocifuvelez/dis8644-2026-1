# sesion-06b Viernes 17 de abril del 2026
### Mantener la calma y el rompecabezas de los transistores 

Llegamos a esta sesión con un objetivo claro: que esto por fin hiciera música. Seguíamos en el plan de ensayo y error, pero tratando de no perder los nervios. Teníamos la esperanza de que, después de todo lo que investigamos, hoy sería el día. 

El descubrimiento de la conmutación: Lo primero fue solucionar el lío de las notas que sonaban todas juntas. Teníamos los transistores 2N2222 ahí en el kit y los vi y dije: "Bueno, para algo puede que nos sirvan". Efectivamente, después de investigar y ver este tutorial de SparkFun, entendimos que funcionaban como "llaves" electrónicas.

¡Fue un alivio gigante ver que el CD4017 por fin empezaba a obedecer! Aprendimos a leer el transistor físicamente: hay que poner la cara lisa hacia una y, desde ahí, identificar los lados. Lo más importante que descubrimos en el montaje fue:

* **La pata del medio (Base):** Es la que recibe la señal del 4017 a través de una resistencia de 100kΩ.
* **La pata derecha (Colector):** Es la que saca la señal hacia el 4093 para activar el oscilador.
* **La pata izquierda (Emisor):** Va conectada directamente a negativo (GND).

Al poner uno a la salida de cada pin del secuenciador, ¡magia!: por fin logramos que cada nota tuviera su propio tiempo y no fuera esa masa de ruido de antes.

Osciladores y Control (CD4093): Luego nos metimos de lleno con el CD4093. Siguiendo la lógica de las compuertas NAND, montamos la etapa donde se genera el sonido. Aquí lo más entretenido (y difícil de cablear) fue integrar los 4 potenciómetros independientes para cada nota. Gracias a esto, podíamos mover las perillas y ver cómo cambiaba el tono de cada paso de la secuencia. Además, mantuvimos el potenciómetro del 555 para controlar la velocidad global del ritmo.

Verificación visual y el consejo del profe: Un truco que nos sirvió mucho para no perdernos fue poner un LED testigo justo en el pin 3 del 555. Así podíamos verificar visualmente si los pulsos de reloj estaban saliendo bien antes de que pasaran al resto del circuito. Si el LED parpadeaba al ritmo que queríamos, sabíamos que la base estaba firme.

La etapa de potencia (LM386): Para el final dejamos la amplificación. El profe nos recomendó algo súper interesante: integrar dos chips LM386 en lugar de uno solo. La idea era dividir la carga y tener una salida dual para que el sonido tuviera más presencia y no saturara tanto un solo componente. Estuvimos un buen rato buscando cómo conectar ambos en esta guía de circuitos de audio, tratando de que los cables no hicieran corto entre las dos protoboards.

Al final, aunque nos dolía la cabeza de tanto revisar cada patita de los chips y el audio final nos dio pelea por temas de continuidad al meterlo en la carcasa, nos fuimos con la frente en alto. Logramos coordinar 4 etapas distintas y entender que la electrónica no es solo seguir un dibujo, sino saber qué hacer cuando el dibujo no suena a la primera.

### Vistazo del proceso
<table>
  <tr>
    <td><img width="500" src="https://github.com/user-attachments/assets/91b6bc2d-39c9-4618-bda1-82fbbe2b536a"></td>
    <td><img width="500" src="https://github.com/user-attachments/assets/351fedf9-4ec8-4ee4-a6aa-86b2b4953cd0"></td>
    <td><img width="500" src="https://github.com/user-attachments/assets/3d74d4aa-12af-49d8-ba17-8d55adab56a7"></td>
    <td><img width="500" src="https://github.com/user-attachments/assets/145c150f-e549-4ee1-b644-05eab4c5b2c9"></td>
    <td><img width="500" src="https://github.com/user-attachments/assets/6fe23965-2bc1-4459-930e-a08c5bebcc0c"></td>
    <td><img width="500" src="https://github.com/user-attachments/assets/67f226f3-bfd6-4543-b7b7-331485352643"></td>
  </tr>
</table>
<video src="https://github.com/user-attachments/assets/f39b6049-b7b6-4d73-ac3b-6709ea3794ad" controls="controls" style="max-width: 600px;"> </video> 

### Referencias complementarias

* Aragón Electrónica. (s. f.). *¿Qué es y para qué sirve el transistor 2N2222?* https://www.aragonelectronica.com  

* Ariat-Tech. (s. f.). *LM386 audio amplifier overview*. https://www.ariat-tech.com  

* Audio Electrónico. (s. f.). *Proyectos de amplificación de audio*. https://www.audioelectronico.com  

* Hackaday. (s. f.). *Logic noise: Sweet oscillator sounds*. https://hackaday.com  

* INCB. (s. f.). *Circuitos con CD4093*. https://www.incb.com  

* Mecatrónica Educativa. (s. f.). *Videos educativos de electrónica* [Canal de YouTube]. https://www.youtube.com/@MecatronicaEducativa  

* Editronikx. (s. f.). *Contenido sobre electrónica digital* [Canal de YouTube]. https://www.youtube.com/@Editronikx  

* Reddit. (s. f.). *Difference between A and B potentiometers (linear vs logarithmic)*. https://www.reddit.com  

* SparkFun Electronics. (s. f.). *Transistors tutorial*. https://learn.sparkfun.com/tutorials/transistors  
