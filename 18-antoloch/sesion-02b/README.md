# sesion-02b
# Apuntes 

##  Personajes destacados
- **Ángel Abusleme**: diseñador electrónico especializado en microelectrónica, microcontroladores y sistemas embebidos.  
- **John Widlar**: ingeniero electrónico pionero en circuitos integrados.  
  - *Dato curioso*: tuvo una cabra para cortar el pasto de su casa.

---

## Ley de Ohm
\[
V = I \cdot R
\]

- **V (voltaje)**: se mide en volts (V).  
- **I (corriente)**: se mide en amperes (A).  
- **R (resistencia)**: se mide en ohmios (Ω).  

---

##   Topología de circuitos
- **Serie**: los componentes se conectan uno tras otro (ejemplo: B–C en serie).  
- **Paralelo**: los componentes comparten los mismos nodos de conexión (ejemplo: BC // DE).  
- **Grafos**: representación visual de conexiones entre puntos.  
- **Caja negra**: se analizan entradas y salidas sin importar el funcionamiento interno.

---

## Componentes electrónicos
- **Resistencias**: limitan la corriente.  
  - Ejemplo: café (1), negro (0), naranjo (3), dorado → 10 kΩ.  
- **Capacitores**:
  - Electrolíticos: polarizados, medidos en µF, con límite de voltaje.  
  - Cerámicos: no polarizados, pequeños y versátiles.  
- **Circuito integrado 555**:
  - 8 patas, numeradas en sentido antihorario desde la muesca.  
  - Usado como temporizador, oscilador y generador de pulsos.  
- **Potenciómetro**: resistencia variable que regula voltaje o corriente.  
- **Fotoresistor (LDR)**: su resistencia depende de la luz; más luz → menor resistencia → parpadeo más rápido.

---

## realizados
- Conectar y desconectar cables en el protoboard para encender un LED.  
- Probar distintos capacitores en el circuito con el 555:
  - 1 µF → parpadeo muy rápido.  
  - 10 µF → parpadeo rápido pero visible.  
  - 100 µF → parpadeo lento.  
- Sustituir una resistencia por un potenciómetro para variar la velocidad del parpadeo.  
- Usar un fotoresistor para que la luz ambiente controle la frecuencia del parpadeo.

---

## Conceptos para no olvidar :)
- **Protoboard**: tablero de pruebas que permite armar circuitos sin soldar.  
- **Polaridad**: fundamental en capacitores electrolíticos y diodos.  
- **Aplicaciones del 555**: temporizadores, osciladores, moduladores de señal, controladores PWM.   
- **Condensadores en osciladores**: determinan la frecuencia de parpadeo del LED.  
- **Código de colores en resistencias**: método estándar para identificar valores sin necesidad de texto.

---

##  Resumen
La clase permitió integrar **teoría básica** (ley de Ohm, topología de circuitos) con **práctica en protoboard**, usando componentes clave como resistencias, capacitores, el CI 555, potenciómetros y fotoresistores.  
Esto sienta las bases para comprender cómo se construyen y controlan los circuitos electrónicos en aplicaciones reales.

