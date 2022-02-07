# JamGDD

# Presentacion
## Nombre de juego
The Choosen number.

## Genero
Juego casual.

# Descripcion
Juego de movil, que esta enfocado a mejorar la memoria.

# Conceptos clave
## Flujo de juego
El juego consiste en que en pantalla saldran un conjunto de numeros de diferentes tamaños y que se moveran por la pantalla el usuario debera tocar
o hacer click en el numero mas alto o en el numero mas bajo segun le indique el inicio de ronda. Habra un tiempo limite para superar cada ronda en caso de que 
el jugador supere el tiempo limite para superar la ronda la ronda sera perdida.

## Progreso
A medida que el jugador pase rondas la cantidad de numeros que saldra por pantalla aumentara, tambien aumentara la diferencia de tamaño entre
ellos asi como la diferencia entre su velocidad de movimiento, aqui estaria una progresion de rondas estandar:

  - Primera Ronda: 
    -  Salen dos numeros que no se mueven.
    -  el mensaje por pantalla es elegir el numero mas alto.
    -  El tiempo para superar la ronda es de 2 minuto.
  - Segunda Ronda: 
    -  Salen 3 numeros, solo uno de ellos se mueve. 
    -  El mensaje por pantalla es elegir el numero mas bajo.
    -  El tiempo para superar la ronda es de 2 minuto.
  - Tercera Ronda: 
    -   Salen 4 numeros, dos de ellos se mueven ambos a distintas velocidades y direcciones.
    -   El mensaje por pantalla es elegir el numero mas bajo.
    -   El tiempo para superar la ronda es de 2 minutos.
  - Cuarta Ronda: 
    -   Salen 5 numeros, todos ellos se mueven en distintas velocidades y direcciones.
    -   el mensaje por pantalla es elegir el numero mas alto.
    -   El tiempo para superar la ronda es de 2 minutos.
  - Quinta Ronda: 
    -   Salen 6 numeros, todos solo 3 de ellos se mueven , ambos 3 a distintas velocidades y direcciones 
    -   El mensaje por pantalla es elegir el numero mas bajo.
    -   El tiempo para superar la ronda es de 2 minutos.
  - Siguientes Rondas: se sigue el mismo patrón que en las rondas anteriores aumentando el numero de numeros que salen por pantalla y variando el numero de numeros
    que se mueven asi como sus velocidades y las direcciones en las que lo hacen. El tiempo disminuira a partir de la ronda 49.

Esta progresión se seguira hasta alcanzar un numero maximo de 50 numeros, dado que mas seria dificil meterlos en pantalla, este numero sera alcanzado en la ronda
49, por lo tanto a partir de esta ronda lo que se hara és aumentar la velocidad a la que se mueven los numeros asi como que cambien de manera aleatoria de direccion
una vez salgan, también se disminuira el tiempo disponible para cada ronda de manera incremental cada 10 rondas superadas, hasta alcanzar un tiempo de 30 segundos a partir
de ahi el tiempo no bajara.

En cada ronda al jugador se le asignara una puntuación dependiendo de lo rapido que haya superado la ronda. En caso de que el jugador se equivoque al elegir el numero, o
se le acabe el tiempo se le restara puntos de su puntuación actual en caso de que la puntuación del jugador sea menor que 0, el juego se reiniciara y pasara a la ronda 1.

El objetivo del juego es alcanzar el maximo de puntos posible.

# Opciones de juego
El progreso del jugador podra ser guardado, o podra empezar desde cero, cada vez que el jugador rompa un record, es decir que alcance una ronda que nunca antes habia alcanzado
se le daran puntos extra, que se le sumara a su puntuacion de partida.
No existira ningun modo de dificultad dado que la dificultad ira aumentado a medida que pase cada ronda, si el jugador es muy bueno alcanzara un numero de ronda mas alta
y por lo tanto una puntuacion mayor, si el jugador és muy malo tendra que repetir la ronda o empezar el juego otra vez en caso de que la puntuación baje de cero, esto 
hara que el jugador tenga que mejorar para pasar a las siguientes rondas , para compensar el esfuerzo de reiniciar el juego se le dara un bonus cada vez que alcance una
ronda que nunca haya alcanzado incrementando mas su puntuación.

# Interfaces
## Interfaz de inicio de ronda
En la interfaz de inicio de ronda se mostrara en pantalla una cuenta atras del 3 al cero y se le informara al jugador si tiene qeu escoger el numero mas bajo o el mas alto, asi
como el tiempo disponible para completar la ronda

## Interfaz pantalla principal
En la interfaz de pantalla principal es donde estara el juego principal apareceran el numero de numeros correspondiente a la ronda, y se moveran conforme se a especificado en el
apartado **Progreso]** de este documento de juego. En la parte superior aparecera un cronometro con el tiempo disponible para acabar la ronda, cuando el tiempo sea menor al 
25% del tiempo inicial dado el cronometro se pondra en rojo.

## Interfaz final Ronda
Cuando finalice la ronda se le mostrara al jugador un icono de OK en caso de que haya ganado o una X en caso de que haya perdido, aparecera el contador de puntos que tiene
el jugador y se activara una animación para mostrar como se incrementan los puntos ganados en la ronda al contador del jugador. Una vez incrementada la puntuación del jugador
en caso de que haya ganado aparecera un boton Siguiente que servira para pasar a la siguiente ronda, y en caso de que haya perdido aparecera un boton Reintentar para reintentar la ronda que no ha conseguido superar.

# Audio
Cada vez que el jugador elija un numero sonara un audio que sera distinto dependiendo de si el jugador ha ganado la ronda o la ha perdido. Tambien habra un sonido de caja 
registradora cada vez que se active la animacion que incrementa los puntos del jugador al final de cada ronda.

# Controles
La unica forma en la que el jugador puede interactuar con el juego es haciendo click, o tocando en caso de que este jugando en dispositivos moviles, esta forma de 
interacción también se aplica a los botones para pasar a la siguiente ronda o para reintentarla.

# Plataformas y dispositivos
Este juego tiene como destino tanto PC como dispositivos moviles, aunque esta enfocado mas al segundo en ambos es jugable, dado que los controles de toque en el dispositivo moviles es el equivalente ha hacer click en un PC.

## Requisitos tecnicos
Practicamente todos los PCs y dispositivos moviles pueden ejecutar el juego, no tiene ningun tipo de exigencia grafica, ni de rendimiento.




