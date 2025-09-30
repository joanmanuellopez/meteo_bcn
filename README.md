# Méteo Barcelona. 1800-2023
### *Análisis de la evolución temporal de la temperatura media y la precipitación anual en la ciudad de Barcelona desde el año 1800 hasta la actualidad*

## Contexto del proyecto
El principal objetivo de este proyecto es practicar el análisis de series temporales, en lenguaje R, a partir de los datos históricos de temperatura y precipitación registradas en la ciudad de Barcelona desde el año 1800. Se quiere visualizar la evolución temporal de los parámetros meteorológicos medidos y descomponer las series temporales resultantes para obtener sus componentes de periodicidad, tendencia y aleatoriedad. Se quiere verificar a partir de representaciones gráficas si hoy en día se está produciendo un aumento de las temperaturas medias, así como si los periodos de sequía o lluvias más escasas son más frecuentes respecto a años anteriores.

* Pregunta 1.
* Pregunta 2.

[Enllaç al projecte](https://public.flourish.studio/story/1789298/)

### Retos

Visualizar los datos disponibles de manera que se puedan hacer observaciones de valor a simple vista. Elegir el rango temporal adecuado para poder ver en una gráfica las tendencias temporales de una manera clara. Cómo hacer ver la información de más de 200 años, con ciclicidad anual en el caso de las temperaturas, en una única gráfica.

### Fuentes de datos
Los datos que se han utilizado en este proyecto se han obtenido de la web del [Servei Meteorològic de Catalunya](https://www.meteo.cat/wpweb/climatologia/dades-i-productes-climatics/serie-climatica-de-barcelona-des-de-1780/) (meteocat). Son dos ficheros de texto plano (.txt) uno con las temperaturas medias (en ºC) y otro con la cantidad de precipitación acumulada (en mm) mes a mes desde 1780 y 1786 respectivamente.

## Conclusiones principales

* El nombre d'habitants en municipis de menys de 3000 habitants decreix en 60000 persones malgrat l'augment notable de població en el global de Catalunya.
* El nombre de municipis de menys de 3000 habitants també decreix, al 2020 n'hi ha 90 menys. El descens de població és menys acusat del que caldria esperar.
* S'observa que la població dels municipis menys poblats l'any 1975, ha crescut més a l'any 2020 en aquells més propers a les ciutats amb més habitants.


## Descripción de los ficheros R

**habitants.R**
Variació del nombre d’habitants als períodes 1975-2020 i 2020-2022. Escriptura dels resultats a dos fitxers csv amb la informació processada.

**dftoviz.R**
Script per a l’adequació dels dataframes processats per a exportar-los a l’eina flourish i mostrar la informació desitjada. [quins csv s’han generat en aquest cas...]

**economics.R**
Script per a la creació d’un fitxer CSV amb la informació del nombre de persones ocupades a cada municipi en funció dels sectors econòmics a data 31 de desembre de 2019

**edats.R**
Script per a la creació d’un fitxer CSV amb la variació d'habitants per grups d’edat a cada municipi al període 2000-2020
