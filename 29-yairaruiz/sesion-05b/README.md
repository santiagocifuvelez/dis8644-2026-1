# sesion-05b

## Apuntes en clase ##

### Chip 4017 ###

![4017](./imagenes/4017.jpg/)

El 4017 es un circuito integrado CMOS de 16 pines que funciona como contador decimal (de 0 a 9).

+ Tiene 10 salidas (Q0 a Q9).
+ Solo una salida está activa a la vez.
+ Cada pulso de reloj hace que avance a la siguiente salida.
  
Funciona típicamente entre 3V y 15V (a veces hasta 18V), lo que lo hace útil en proyectos electrónicos simples como secuenciadores.

### Funcionamiento básico ###

El 4017 avanza con cada pulso que recibe en el pin de reloj:

+ Llega un pulso - se activa Q0
+ Llega otro - se activa Q1
+ Luego Q2, Q3…
+ Hasta Q9
+ Después vuelve a Q0 y repite el ciclo
  
En el fondo, cuenta impulsos y distribuye la señal entre sus salidas.

### Relación con el clock (reloj) ###

El 4017 necesita un clock para funcionar.

El clock es una señal de pulsos que define el ritmo del sistema:

+ Más rápido → secuencia más rápida
+ Más lento → secuencia más lenta
  
Este clock se puede generar con:

+ Chip 555
+ Chip 4093

### “Secuenciadores” ###

El 4017 se usa mucho como secuenciador, porque activa salidas una por una en orden.

Esto permite crear patrones, por ejemplo:

+ Luces que se encienden en secuencia
+ Ritmos electrónicos
+ Activación de distintos módulos

Es como un sistema que “recorre” sus salidas siguiendo el ritmo del clock.
