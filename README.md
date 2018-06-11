# ATPstatistics-cleaning
Estadísticas de los resultados de partidos de tenis ATP

La Asociación de Tenistas Profesionales (ATP) organiza diferentes torneos en una misma temporada, que abarca de Enero a Noviembre. Los torneos se clasifican según la puntuación que el ganador recibe en cada uno de ellos:

- ATP 250
- ATP 500
- ATP 1000
- Grand Slam (2000)

Por lo tanto, los ganadores se embolsan desde 250 puntos en el primero torneo hasta los 2000 de un Grand Slam. Esta puntuación se utiliza para realizar la clasificación de los tenistas en el ranking mundial. Los tenistas con mejor ranking disponen de plazas directas para jugar los torneos, mientras que el resto tendrá que jugar un mini torneo para poder acceder a ellos.

Además de la puntuación, los torneos difieren en la cantidad de tenistas que participan en ellos, diferencia que va desde los 28 tenistas que disputan un ATP 250 hasta los 128 de un Grand Slam.

El dataset "ATPStatistics" utilizado para esta práctica, es un set de datos sobre la competición ATP World Tour que se ha obtenido mediante un proyecto de web Scraping de la página http://www.atpworldtour.com/ desarrollado por Alejandro Manuel Olivares Luque.

En dicho proyecto se ha realizado la extracción de datos, estadísticas y resultados de los partidos oficiales organizados por Asociación de Tenistas Profesionales (ATP).

El desarrollo del scrapper se ha realizado mediante el lenguaje Python y haciendo uso de librerías adicionales como urllib2, beautifulsoup y xlwt. Todo el código se encuentra disponible en Github en el siguiente enlace: https://github.com/olivaresluque/scrapATP

El resultado obtenido se ha almacenado en fichero de Microsoft Excel en formato xls. En él se ha volcado la información relativa a los partidos comprendidos entre el año 2011 y la actualidad, lo que representa algo más de 30.000 registros. Para cada registro se dispone de los siguientes atributos:

- id_partido: Código identificador únido del partido
- Player 1: Nombre del jugador 1 del partido
- Player 2: Nombre del jugador 2 del partido
- Serve Rating 1: Puntuación oficial del saque para el jugador 1
- Serve Rating 2: Puntuación oficial del saque para el jugador 2
- Aces 1: Cantidad de ACEs del jugador 1 en el partido	
- Aces 2:  Cantidad de ACEs del jugador 2 en el partido
- Double Faults 1: Número de faltas dobles del jugador 1 en el partido
- Double Faults 2: Número de faltas dobles del jugador 2 en el partido
- % 1st Serve 1: Porcentaje de servicios correctos en el primer servicio para el jugador 1
- % 1st Serve 2: Porcentaje de servicios correctos en el primer servicio para el jugador 2
- % 1st Serve Won 1: Porcentaje de puntos ganados con el primer servicio para el jugador 1
- % 1st Serve Won 2: Porcentaje de puntos ganados con el primer servicio para el jugador 2
- % 2nd Serve Won 1: Porcentaje de puntos ganados con el segundo servicio para el jugador 1
- % 2nd Serve Won 2: : Porcentaje de puntos ganados con el segundo servicio para el jugador 2
- % Break Point Saved 1: Porcentaje de puntos de break salvados por el jugador 1
- % Break Point Saved 2: Porcentaje de puntos de break salvados por el jugador 2
- Served Games Played 1: Número de juegos en los que ha tenido servicio el jugador 1
- Served Games Played 2: Número de juegos en los que ha tenido servicio el jugador 2
- Return Rating 1: Puntuación oficial de resto para el jugador 1
- Return Rating 2: Puntuación oficial de resto para el jugador 2
- % 1st Serve Return Won 1: Porcentaje de puntos ganados restando el primer servicio por el jugador 1
- % 1st Serve Return Won 2: Porcentaje de puntos ganados restando el primer servicio por el jugador 2	
- % 2nd Serve Return Won 1: Porcentaje de puntos ganados restando el segundo servicio por el jugador 1
- % 2nd Serve Return Won 2: Porcentaje de puntos ganados restando el segundo servicio por el jugador 2
- % Break Point Converted 1: Porcentaje de puntos de break convertidos por el jugador 1
- % Break Point Converted 2: Porcentaje de puntos de break convertidos por el jugador 2
- Return Games Played 1: Número de juegos en los que ha restado el jugador 1
- Return Games Played 2: Número de juegos en los que ha restado el jugador 2
- % Served Point Won 1: Porcentaje de puntos ganados con su servicio para el jugador 1
- % Served Point Won 2: Porcentaje de puntos ganados con su servicio para el jugador 2
- % Return Point Won 1: Porcentaje de puntos ganados con su resto para el jugador 1
- % Return Point Won 2: Porcentaje de puntos ganados con su resto para el jugador 2
- % Total Point Won 1: Porcentaje total de puntos ganados por el jugador 1
- % Total Point Won 2: Porcentaje total de puntos ganados por el jugador 2
- Winner: Nombre del ganador del partido
- Tournament: Nombre del torneo
- Started date: Fecha de inicio del torneo
- Ended date: Fecha de fin del torneo
- Surface: Superficie del torneo

La extracción de estos datos tiene como objetivo crear un almacén de datos con el que realizar un estudio estadístico y construir un modelo de clasificación que permita predecir el ganador de nuevos partidos o torneos.
