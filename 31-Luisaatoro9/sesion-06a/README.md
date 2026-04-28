# sesion-06a Martes 14 de abril del 2026
Esta sesión fue el puntapié inicial para poner en marcha todo lo que veníamos aprendiendo de forma teórica en las clases anteriores. Pasar de ver los componentes sueltos a intentar armar este "monstruo" de 4 chips (555, 4017, 4093 y LM386) fue un choque de realidad. Empezamos analizando el esquema técnico para entender cómo se conectaban las etapas, pero la práctica fue otra historia.

Investigación de los Chips: Para no quemar todo (aunque igual nos pasó), nos pusimos a investigar qué hacía realmente cada integrado que nos entregaron. Pasamos mucho tiempo en el lab pegadas al celu viendo datasheets y tutoriales:

* **El Reloj (NE555):** Investigamos cómo generar la señal de clock. Aprendimos que el 555 es el estándar para esto. Vimos este recurso de Circuit Digest sobre el NE555 para entender cómo el capacitor y la resistencia definen la velocidad del pulso.
* **El Contador (CD4017):** Buscamos cómo repartir ese pulso en 4 pasos. Encontramos este video de Electronic Clinic que nos enseñó a usar el pin 15 (Reset) para que la secuencia no se fuera hasta 10, sino que volviera a empezar en el 4.

El proceso de error: Fue frustrante al principio... Estábamos tan ansiosas que cometimos errores básicos: quemamos varios LEDs por no ponerles resistencia o por conectarlos al revés. También nos pasaba que el circuito no hacía nada porque nos faltaban puentes críticos a negativo (GND). Aprendimos a la mala que si una pata del chip no tiene su tierra bien puesta, todo el sistema falla. Terminamos la sesión con una maraña de cables y la sensación de que, aunque investigamos mucho, la protoboard tiene su propia maña.

### Vistazo del proceso
<video src="https://github.com/user-attachments/assets/b50706b1-4832-4d3f-8707-4420486927ce
" width="600" controls> </video> 
<video src="https://github.com/user-attachments/assets/3568d48e-7871-4df1-9749-429f20abdf90" width="600" controls> </video> 
<p align="center"> <img src="https://github.com/user-attachments/assets/b7d43e45-b501-4281-bea5-03e99a60bdd0" width="320" /> <img src="https://github.com/user-attachments/assets/73b2c146-6b03-450b-b111-d7c3e895f913" width="320" /> </p> 

**Además de los circuitos integrados, nos abastecimos con protoboards, jumpers (cables) y otros componentes pasivos necesarios para el ensamblaje y las pruebas del circuito.**

Nota técnica: El pin 13 (Clock Enable) del IC 4017 debe estar conectado a tierra (GND) para habilitar la recepción de pulsos de reloj. Si este pin se encuentra en estado alto o flotante, el contador se inhabilita, impidiendo el avance de la secuencia.

Algo tambien importante entre protoboard siempre conectar a positivo y negativo, se nos olvidaba mucho alimentar de energia a las protoboards que estaban con un chips aparte en las pruebas que fuimos haciendo al principio. 

## Referencias

* Circuit Digest. (s. f.). *555 timer astable multivibrator circuit diagram*. https://circuitdigest.com/electronic-circuits/555-timer-astable-multivibrator-circuit-diagram  

* Circuit Digest. (s. f.). *555 timer bistable multivibrator circuit diagram*. https://circuitdigest.com/electronic-circuits/555-timer-bistable-multivibrator-circuit-diagram  

* Circuit Digest. (s. f.). *555 timer IC*. https://circuitdigest.com/article/555-timer-ic  

* Circuit Digest. (s. f.). *555 timer monostable circuit diagram*. https://circuitdigest.com/electronic-circuits/555-timer-monostable-circuit-diagram  

* Editronikx. (2015, junio 29). *Como funciona el CD4017 | Teoria y practica* [Video]. YouTube. https://www.youtube.com/watch?v=0ExlyDGlqZc  

* El profe García. (2014, mayo 21). *Contador con el 4017 y 555 - Luces de auto fantástico* [Video]. YouTube. https://www.youtube.com/watch?v=p2tBTxzbOeM  

* Eleccircuit. (s. f.). *IC 4017 datasheet*. https://www.eleccircuit.com/ic-4017-datasheet/  

* Mecatrónica Educativa. (2015, agosto 30). *Tutorial: Circuito integrado 555 (parte 1: introducción)* [Video]. YouTube. https://www.youtube.com/watch?v=Z6WqBp4w0sE  

* Mecatrónica Educativa. (2015, octubre 14). *Tutorial: Circuito integrado 555 (parte 2: modo monostable)* [Video]. YouTube. https://www.youtube.com/watch?v=oqKeS-uJpj0  

* Morales, L. Q. (s. f.). *Circuito integrado 555 y 4017* [Presentación]. Prezi. https://prezi.com/rtr7hgq0h2v_/circuito-integrado-555-y-4017/  
