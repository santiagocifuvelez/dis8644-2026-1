# sesion-06b

# Apuntes 17/04

## Fe de Erratas!!

Misa hizo las siguientes modificaciones en el esquemático que vimos la clase pasada ya que habían unos problemas:

1. Estabilizador de CLOCK (555): Se añadió un ``R Pull Down`` de 100k entre el pin 3 del 555 y el pin 14 del 4017 (ojo, éste debe estar cerca del 14).
2. Condensador de desacople: Se agrega un 104 en cada pin de alimentación de todos los chips (cerca de éste).
3. Condensador de acople: En el potenciómetro que está entre el MIX y el 386, se añade un condensador de 100 µF que va conectado al pin 2 del potenciómetro.
4. Buscar fuentes de ``Va`` alternativas: En el caso de 12V, sirven las baterías de autos y los paneles solares. En el caso de 9V, sirven nuestras baterías. En el caso de 5V, sirven los USB-A (podemos conectarnos a una micro roja jiji).

Luego de informarnos sobre los cambios que hubieron, nos dieron la clase para poder trabajar en lograr sonar, por lo que con mi grupo nos fuimos al LID con toda la intención de finalmente poder hacer ruido, es decir, lograr que funcione el circuito entero. Cuando llegamos al LID, empezamos a trabajar de manera inmediata y aplicamos los cambios que se nos mencionaron.
