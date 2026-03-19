# sesion-02a

### Circuito LED básico

![primer-circuito](./imagenes/circuito.jpg)

### Circuito LED paralelo

![circuito-paralelo](./imagenes/circuito-paralelo.jpg)

---

## Apuntes clases

Se nos entregaron los materiales en una caja, la cual traía dos potenciómetros B100k, cables Dupont, una protoboard, un parlante, cuatro chips, un broche de batería, 10 resistencias de 220, 10 resistencias de 1000, y una batería de 9v.

Aprendimos a identificar los valores de los colores que hay en las potencias que nos dieron, y cómo se leen en conjunto:

- Negro = 0
- Café = 1
- Rojo = 2

Los colores se leen de un lado a otro, y para poder identificar la dirección nos guiamos por el dorado que siempre suele ser el último, indicando el porcentaje.
Los primeros dos colores son los primeros dos dígitos, mientras que el tercer color es la cantidad de ceros, por ejemplo, rojo-rojo-café-dorado es igual a 220 Ω, ya que el rojo equivale a 2, y el café a 1, indicando que solo hay un cero.

### Circuitos

Se nos mostraron ejemplos de circuitos en la pizarra para enseñarnos que no solo existen los circuitos básicos, sino que también están los paralelos, en donde los LED son independientes. Aparte, se nos mostró que hay distintas maneras en las que se puede representar la batería, la cual no necesariamente tiene que estar como un solo símbolo, sino que se puede separar a los dos extremos como 9v y 0v.

---

### Encargo LQXTLC (Lo Quito X Ti, Lo Coloco)

#### Primer circuito

![primer circuito](./imagenes/LQXTLC-1.jpg)

| loquitoportilocoloco | D1  | D2  | D3  | D4  |
| ---                  | --- | --- | --- | --- |
| R1                   |  0  |  0  |  0  |  0  |
| R2                   |  1  |  0  |  0  |  1  |
| R3                   |  1  |  1  |  1  |  0  |
| R4                   |  1  |  1  |  1  |  0  |
| R5                   |  1  |  0  |  0  |  1  |

#### Segundo circuito

![segundo circuito](./imagenes/LQXTLC-2.jpg)

| loquitoportilocoloco | D1  | D2  | D3  |
| ---                  | --- | --- | --- |
| R1                   |  1  |  0  |  1  |
| R2                   |  1  |  0  |  1  |
| R3                   |  1  |  0  |  1  |
| R4                   |  1  |  0  |  1  |
| R5                   |  0  |  1  |  1  |
| R6                   |  1  |  1  |  1  |
| R7                   |  1  |  1  |  1  |
| R8                   |  1  |  1  |  0  |

#### Tercer circuito

![tercer circuito](./imagenes/LQXTLC-3.jpg)

| loquitoportilocoloco | D1  | D2  | D3  | D4  |
| ---                  | --- | --- | --- | --- |
| R1                   |  1  |  1  |  1  |  1  |
| R2                   |  1  |  1  |  1  |  1  |
| R3                   |  1  |  1  |  0  |  1  |
| R4                   |  1  |  0  |  1  |  0  |
| R5                   |  1  |  1  |  1  |  1  |
| R6                   |  1  |  1  |  1  |  1  |

---

### Encargo artistas

#### Kraftwerk

Escuché el álbum Die Mensch-Maschine, publicado el 19/05/1978. Al inicio estaba escuchando la versión en inglés, pero al terminar el álbum se empezó a reproducir la versión en alemán, la cual encontré aún más interesante ya que no podía entender lo que decían y de igual manera sonaba agradable.

La canción Spacelab entre los primeros 40 segundos me recordó por un momento al álbum Mother Earth's Plantasia (1976), pero puede que sea sólo por el juego en loop que hace con las notas de bajas a altas y su velocidad. Otra cosa que se me hizo curioso es como en todo el disco cantan con voces robóticas, pero se hace la excepción en Das Model y en Neonlicht en donde usan la voz humana.

![Portada del álbum](./imagenes/die-mensch-maschine.jpg)

La portada está inspirada en el artista ruso El Lissitzky y en el movimiento supremacista. En la fotografía tomada por Gunther Frohling, los integrantes estaban usando camisas rojas y corbatas negras, lo cual daba pistas sobre la critica al comunismo ruso que usó al proletariado de manera poco humana, pareciendo robótica y dominada. Ésto también se puede observar en las presentaciones en vivo, en donde los integrantes se van alejando de sus puestos en el escenario y son reemplazados por los muñecos robots, copias de ellos mismos. En la última canción del álbum, Die Mensch-Maschine, se repite en todo momento "die mensch-maschine", con una voz robótica, demostrando así el como el hombre tiene que trabajar de manera mecánica, al igual que una máquina, sin tener como opción el poder distinguirse de los demás.
