# AVIATION SAFETY NETWORK DATA

## DESCRIPCION GENERAL

Este repositorio contiene el scraping realizado a la base de datos: https://aviation-safety.net/database/

Actualmente el dataset resultante abarca *1919* hasta el *18 de Mayo del 2023.* Contiene 20711 registros con 30 campos.

No se encontro otro notebook por internet que hiciese lo propio.

El unico repositorio similar pero no igual que encontre es el siguiente: https://github.com/alsonpr/Aviation-Safety-Network-Dataset. 

### DIFERENCIAS CON OTROS

(1)

Mi dataset es el resultado de cada uno de los incidentes/accidentes para cada año. No la tabla asociada a cada año.
Para que se entienda la diferencia, el archivo json con el que puedes importar la data usando pandas, **tiene 21 columnas mas.** Pero, no solamente eso, ya que dentro de cada columna se pueden crear otros campos. Por ejemplo:

En la columna crew o passengers uno se encuentra data referentes la cantidad de fallecidos como a la cantidad de ocupantes.

Otro caso, es la columna narrativa, la cual, tiene textos de hasta 16823 caracteres para extraer informacion relevante.

Por lo que el numero de columnas es mucho mayor a 30.

(2)

Este notebook, no solo tiene el dataset con la data asociada a cada accidente, sino que tiene los links asociados a cada accidente. Por lo que es facilmente actualizable y/o modificable. Supongamos que queres extraer mas informacion, como la imagen asociada al incidente, puedes adaptar facilmente este codigo para lograr dicho objetivo.

(3)

Este notebook, incluye el web-scraper asociado. De este modo, asociandolo con lo anterior, te permite re-adaptar el codigo a tu situacion o gusto. Sin embargo, ten presente, que en mi caso particular, al codigo le tomo las mas de 20 links asociados, alrededor de 5 horas. Fui y volvi del GYM, merende, me bañe, y cague tambien (si, me tomo 5 horas eso, cago despacio).

### DEFINICION DE COLUMNAS

Se puede encontrar informacion referente a las columnas en este link provisto por **Aviation Safety Network**:

https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Faviation-safety.net%2Fabout%2FASN-standards.doc&wdOrigin=BROWSELINK

## TECNOLOGIAS

Utiliza las librerias de:
- Selenium
- CSV
- JSON
- Google Chrome + WebDriver asociado.

Lo intente realizar con BeautifulSoup4 y no me dejo.

## NOTAS FINALES

Este mini-proyectito surgio a partir del proyecto 02 de la etapa labs del bootcamp de SoyHenry.

En este proyecto 02 habia que realizar un analisis sobre accidente de aviones. Para complementar el dataset brindado por ellos, se realizo esto.

Este analisis sobre accidente de aviones, tambien se encuentra en mi cuenta de github jcamatta por si queres chequearlo.

Si lo utilizas, me encantaria que citaras el repositorio.

Me encantaria mas que lo modificaras.

Adios bella/o.
