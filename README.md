![Player_3pts.png](images/Player_3pts.png)


# Proyecto ETL y Visualización
## Introducción:


En el siguinte proyecto se me ha encargado como objetivo extraer datos de 3 fuentes diferentes y utilizando varias tecnicas de extranción, para a posteriori tranformarlos, cargarlos a una base de datos Y por último realizar una análisis con su correspondiente visualización.

El tema que he escogido es la NBA, más en particular estadísticas completas de los partidos desde el año 2004 hasta el 2020. Para ello utilizaré diferentes fuentes, en una de ellas descargaré directamente archivos en csv, otra será una API y por último scrapearé una web.

En cuanto al análisis y visualización utilizaré Tableau con el que realizaré varios dashboards en los que se muestren diferentes perspectivas de los datos.



## Fuentes de los datos:

 - https://www.kaggle.com/datasets/nathanlauga/nba-games
 - https://www.balldontlie.io/#get-all-players
 - https://en.wikipedia.org/wiki/List_of_United_States_cities_by_population
 - https://espndeportes.espn.com/basquetbol/
 

## Objetivos:

- Recopilar datos de 3 fuentes y 3 técnicas de extracción. 
- Explorar, limpiar y transformar los datos.
- Diseñar, crear y alimentar la base de datos.
- Analizar y visualizar.


## Entregables:

- `nba_stats.sql` 
- `nba_stats.twb`


## Extracción de datos:

Como primera fuente de datos utilizo la web de kaggle, en la que me descargo una serie de archivos de csv que serán el punto de partida de mi base de datos, entre ellos se encuentran estadisticas de partidos por equipos e individualizada por jugadores.

Otra de las fuentes de datos es la api de balldontlie, en la que extraeré ayudandome de la biblioteca request de datos de los jugadores como posición, estatura y peso.

Por último en wikipedia mediante scrapeo a través de Selenium me haré con una tabla de información sobre las ciudades de Estados Unidos.
        


## Exploración, limpieza y transformación:

Comienzo importando todos los csv a un jupyter notebook y los guardo como dataframes de pandas para revisar los datos. Hago lo mismo con los json procedentes de la api y con la tabla extraida del scrapeo 

Continuo limpiando y gestionando los datos nulos, modificando y cambiando el tipo de datos y uniendo alguna de tablas.



## Diseño y creación de la base de datos:


Primero me diseño la estructura de la base de datos en un papel y cuando tengo claro cuales son las primary y foreign keys de cada tabla me dispongo a generarla en mySQL

Para ello utilizo otra vez jupyter nootebook y me ayudo de mysql-conector para realizarlo de forma automatizada. Primero creo la base de dato, luego las tablas con sus relaciones y por último le inserto los datos.

## Analizar y visualizar:

Como seguidor de la NBA he visto la evolución de la forma de jugar en las dos últimas decadas, en la que aparentemente cada vez se tira mas de 3 puntos y menos de 2 puntos. Con este análisis, comprobares si los datos contrastan mi percepción.

Para ello lo primero que compruebo es la evolución en el tiempo del número de tiros de 3 y 2 puntos en toda la liga y se aprecia lo siguiente:

- La tendencia del tiro de 3 puntos va en aumento desde el 2004, se hace mucho mas significativa con los años a partir de 2010
- La tendencia del tiro de 2 puntos se mantiene estable desde el 2004 y empieza a decrecer paulatinamente a partir del 2010.

Esto me lleva a pensar que efectivamente desde el 2004 cada vez se recurre al tiro de 3 y desde 2010 algunos equipos basan su juego en esta táctica. Por lo que el siguiente paso es estudiar la tedencia indivial de los equipos que mas tiran y para identificar a los mas influyentes:

- Houston Rocket
- Golden State Warriors

Realizo el mismo ejercicio para determinar los jugadores mas influyentes:

- Stephen Curry
- James Harden 
- Klay Thompson
- Damian Lillard



## Enlaces y Recursos:


- <https://numpy.org/doc/1.18/>
- <https://pandas.pydata.org/>
- https://docs.python.org/3/library/functions.html
- https://plotly.com/python/
- https://matplotlib.org/
- https://seaborn.pydata.org/
- https://pandas.pydata.org/docs/
- https://docs.python-requests.org/en/latest/
- https://dev.mysql.com/doc/connector-python/en/
- https://selenium-python.readthedocs.io/
- https://www.tableau.com/es-es





```python

```



```python

```
