# sesion-05a

Las señales binarias son la forma más básica de representar información en electrónica digital.

Solo utilizan dos estados:

- 0 → sin voltaje (conectado a tierra)
- 1 → con voltaje (por ejemplo, 9V)
  
En lugar de valores continuos, todo se reduce a encendido o apagado.

Cuando este cambio entre 0 y 1 ocurre muchas veces por segundo, se genera una señal repetitiva. Si el cambio es brusco, se forma una onda cuadrada, que en algunos casos puede transformarse en sonido.

---

### VCV RACK

Es un programa para armar sintetizadores virtuales, basado en módulos que se conectan entre sí.

- Las conexiones de entrada y salida están marcadas visualmente
- El gate actúa como un interruptor que deja pasar o corta la señal

- VC: algo que se controla mediante voltaje
- VCO: genera las ondas (sonido)
- LFO: modifica parámetros lentamente (no se escucha como tono principal)
- VCA: regula la intensidad del sonido
- VCF: cambia el color o carácter del sonido

---

### Formas de onda

- Seno: sonido puro, sin componentes extra
- Triángulo: parecido al seno, pero con más contenido armónico
- Cuadrada: sonido más artificial, típico de consolas antiguas
- Sierra: muy rica en armónicos, más agresiva

---

### Operadores y compuertas lógicas

Las compuertas lógicas permiten tomar decisiones dentro de un circuito usando valores binarios (0 y 1).

- AND → solo entrega 1 si ambas entradas están en 1
- OR → entrega 1 si al menos una entrada es 1
- NOT → cambia el valor (de 1 a 0 o de 0 a 1)
- XOR → da 1 cuando las entradas no coinciden
- NAND → es lo opuesto a AND (solo da 0 cuando ambas son 1)

--- 

### Chip 4093

El 4093 es un circuito integrado usado en electrónica digital. Contiene 4 compuertas NAND en un solo chip.

### Características principales

- Funciona con lógica binaria (0 y 1)
- Cada compuerta es del tipo NAND
  
Incluye Schmitt Trigger, lo que ayuda a:
- Limpiar señales inestables
- Evitar errores cuando la señal no es totalmente clara

### Alimentación

- Pin 14 → VCC (voltaje, por ejemplo 9V o 5V)
- Pin 7 → GND (tierra)
  
Cada compuerta tiene 2 entradas y 1 salida:

### Compuerta 1
Pin 1 → Entrada A

Pin 2 → Entrada B

Pin 3 → Salida

### Compuerta 2

Pin 5 → Entrada A

Pin 6 → Entrada B

Pin 4 → Salida

### Compuerta 3

Pin 8 → Entrada A

Pin 9 → Entrada B

Pin 10 → Salida

### Compuerta 4

Pin 12 → Entrada A

Pin 13 → Entrada B

Pin 11 → Salida
