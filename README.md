# JamGDD

# Descripcion
Juego de movil, que esta enfocado a mejorar la memoria.

# Flujo de juego
El juego consiste en que en pantalla saldran un conjunto de numeros de diferentes tamaños y que se moveran por la pantalla el usuario debera tocar
o hacer click en el numero mas alto o en el numero mas bajo segun le indique el inicio de ronda.

# Progreso
A medida que el jugador pase rondas la cantidad de numeros que saldra por pantalla aumentara, tambien aumentara la diferencia de tamaño entre
ellos asi como la diferencia entre su velocidad de movimiento, aqui estaria una progresion de rondas estandar:

  - Primera Ronda: Salen dos numeros que no se mueven , (el mensaje por pantalla es elegir el numero mas alto). 
  - Segunda Ronda. Salen 3 numeros, solo uno de ellos se mueve, (el mesnaje por pantalla es elegir el numero mas bajo).
  - Tercera Ronda: Salen 4 numeros, dos de ellos se mueven ambos a distintas velocidades y direcciones (el mesnaje por pantalla es elegir el numero mas bajo).
  - Cuarta Ronda: Salen 5 numeros, todos ellos se mueven en distintas velocidades y direcciones (el mensaje por pantalla es elegir el numero mas alto).
  - Quinta Ronda: Salen 6 numeros, todos solo 3 de ellos se mueven , ambos 3 a distintas velocidades y direcciones (el mensaje por pantalla es elegir el numero mas bajo):
  - Siguientes Rondas: se sigue el mismo patrón que en las rondas anteriores aumentando el numero de numeros que salen por pantalla y variando el numero de numeros
    que se mueven asi como sus velocidades y las direcciones en las que lo hacen.

Esta progresión se seguira hasta alcanzar un numero maximo de 50 numeros, dado que mas seria dificil meterlos en pantalla, este numero sera alcanzado en la ronda
49, por lo tanto a partir de esta ronda lo que se hara és aumentar la velocidad a la que se mueven los numeros asi como que cambien de manera aleatoria de direccion
una vez salgan.

En cada ronda al jugador se le asignara una puntuación dependiendo de lo rapido que haya superado la ronda. En caso de que el jugador se equivoque al elegir el numero
se le restara puntos en caso de que la puntuación del jugador sea menor que 0, el juego se reiniciara y pasara a la ronda 1.

El objetivo del juego es alcanzar el maximo de puntos posible.

# Opciones de juego
El progreso del jugador podra ser guardado, o podra empezar desde cero, cada vez que el jugador rompa un record, es decir que alcance una ronda que nunca antes habia alcanzado
se le daran puntos extra, que se le sumara a su puntuacion de partida

# Interfaces
## Interfaz de inicio de ronda
En la interfaz de inicio de ronda se mostrara en pantalla una cuenta atras del 3 al cero y se le informara al jugador si tiene qeu escoger el numero mas bajo o el mas alto

## Interfaz pantalla principal
En la interfaz de pantalla principal es donde estara el juego principal apareceran el numero de numeros correspondiente a la ronda, y se moveran conforme se a especificado en el
apartado Progreso de este documento de juego.

## Interfaz final Ronda
Cuando finalice la ronda se le mostrara al jugador un icono de OK en caso de que haya ganado o una X en caso de que haya perdido, aparecera el contador de puntos que tiene
el jugador y se activara una animación para mostrar como se incrementan los puntos ganados en la ronda al contador del jugador. Una vez incrementada la puntuación del jugador
en caso de que haya ganado aparecera un boton Siguiente que servira para pasar a la siguiente ronda, y en caso de que haya perdido aparecera un boton Reintentar para reintentar la ronda que no ha conseguido superar.



