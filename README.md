# Méteo Barcelona. 1800-2023
### *Análisis de la evolución temporal de la temperatura media y la precipitación anual en la ciudad de Barcelona desde el año 1800 hasta la actualidad*

## Contexto del proyecto
El principal objetivo de este proyecto es practicar el análisis de series temporales, en lenguaje R, a partir de los datos históricos de temperatura y precipitación registradas en la ciudad de Barcelona desde el año 1800. Se quiere visualizar la evolución temporal de los parámetros meteorológicos medidos y descomponer las series temporales resultantes para obtener sus componentes de periodicidad, tendencia y aleatoriedad. Con el análisis exploratorio y las gráficas generadas se pretende dar resupesta a dos cuestiones:

* La temperatura media anual, ¿tiende a aumentar más en los últimos años?
* Los periodos de sequías o lluvias más escasas, ¿son más frecuentes respecto a años anteriores?

### Retos

Transformar la escala temporal proporcionada en el dataset original, mensual, para visualizar de manera adecuada los datos disponibles y poder hacer observaciones de valor a simple vista. Esto implica elegir el rango temporal adecuado para poder ver en una gráfica las tendencias temporales de una manera clara, que permita ver la información recopilada durante más de 200 años de manera rápida y sencilla.

### Fuentes de datos
Los datos que se han utilizado en este proyecto se han obtenido de la web del [Servei Meteorològic de Catalunya](https://www.meteo.cat/wpweb/climatologia/dades-i-productes-climatics/serie-climatica-de-barcelona-des-de-1780/) (meteocat). Son dos ficheros de texto plano (.txt) uno con las temperaturas medias (en ºC) y otro con la cantidad de precipitación acumulada (en mm) mes a mes desde 1780 y 1786 respectivamente.

## Conclusiones principales

### Consideraciones previas
En este proyecto se ha puesto de manifiesto la importancia de usar una escala temporal adecuada para observar tendencias. Por ejemplo:
* El paso de la escala mensual a una escala anual, y la agrupación de los datos en periodos de cinco años, ha permitido visualizar a simple vista tendencias climatológicas en la ciudad de Barcelona en un periodo de más de 200 años.

### Observaciones a partir del análisis
* La temperatura media anual en los últimos años ha experimentado un aumento más acusado.
* La precipitación anual media en los últimos años inferior a la media global del periodo desde el año 1800.
  * No obstante, se ha observado un periodo de siete quinquenios, entre 1805 y 1839, en los que la precipitación media anual es inferior a la media global.

* La descomposición de la serie temporal de la temperatura de los últimos diez años pone de manifiesto la periodicidad anual de esta magnitud, así como la tendencia a la alza de los últimos dos años.
* La descomposición de la serie temporal de la precipitación da una idea del régimen irregular de las lluvias típicas del clima mediterráneo
  * A pesar de esta irregularidad, se detecta una mayor ocurrencia de estas lluvias en primavera y otoño.

## Descripción de los ficheros R

Se incluye el fichero RMD que se usa para generar el informe en HTML.

**Main.Rmd**
El fichero se estructura en las siguientes secciones:  
* Introducción.
* Obtención y adecuación de los datos. Análisis exploratorio.
* Análisis de las series temporales en el periodo 1800-2023
* Conclusiones.
