## **Nota metodológica de indicadores por Estado**

Por Grissel Olivera Martínez

Desde mediados marzo de 2020 un grupo de 32 estudiantes del Tecnológico
de Monterrey han revisado notas periodísticas de los medios locales más
importantes de cada entidad federativa con la intención de dar
seguimiento a la evolución de la pandemia por COVID-19 así como sus
efectos económicos y sociales e identificar las estrategias de gobiernos
locales y ciudadanía para hacer frente a esta enfermedad.

Para capturar la riqueza de la información se diseñó el instrumento que
denominamos ¿Quién es quién en los estados? Y como resultado se obtuvo
una base de datos con 79 variables de la cual se construyeron 14
indicadores que reflejan el comportamiento de los estados en las
siguientes temáticas:

**1.** Medidas de Aislamiento: esta sección consta de 12 variables que
indican si en los estados se decretó el cierre obligatorio de lugares de
trabajo, convivencia social, lugares de culto como cafés y restaurantes,
oficinas, iglesias, comercio, bancos, maquilas, cancelación de obras de
la construcción, etc; asimismo se incluyó una pregunta sobre planes de
reactivación económica en las maquilas.

***1.b*** Medidas de aislamiento llevadas a cabo por ciudadanía u
organizaciones del sector privado: al igual que la sección anterior se
busca identificar a través de 6 variables las iniciativas de aislamiento
llevadas a cabo por la ciudadanía sin necesidad de que el gobierno las
haya decretado tales como: revisión en las carreteras de entrada y
salida a sus comunidades, bloqueos a automóviles de fuera; cierre de
sucursales bancarias, maquilas y obras de construcción, así como
sanitización en mercados y/o centrales de abasto.

**2.** Seguridad: este apartado contiene 10 ítems para capturar los
efectos sociales derivados de la pandemia como saqueos a comercios,
hostilidad hacia el personal de salud, violencia familiar, agresiones
hacia el personal de seguridad en los hospitales y vecinos contagiados
y, también, contiene las estrategias para mantener el orden como
operativos y patrullajes e implementación de multas.

**3.** Transparencia y Comunicación: Esta sección cuenta con 11
variables relacionadas con la capacidad de respuesta de los estados para
mantener informada a la ciudadanía acerca de la evolución de la pandemia
en sus estados; los esfuerzos por desarrollar innovaciones tecnológicas
como aplicaciones para informar o detectar de síntomas; así como la
presencia de actos de corrupción o desacuerdos con la federación en
cuanto a las estrategias para manejar la pandemia.

**4.** Salud Pública: La sección de salud pública a su vez se divide en
dos apartados. El primero (apartado a) consta de 13 variables
relacionadas con carencias de insumos, equipos o saturación del sistema
de salud y de las acciones para abastecer dichas necesidades. El segundo
(aparatado b) contiene 11 preguntas para identificar las estrategias del
gobierno y las empresas para ayudar a manejar la pandemia, éstas van
desde reconversión de espacios ante la saturación de hospitales,
selección de hospitales para atender únicamente a pacientes contagiados
por COVID-19, aplicación de pruebas, colaboración con hospitales
privados, manejo de albergues, donaciones de plasma, etc.

**5.** Economía: Este apartado tiene 14 variables que capturan las
iniciativas de apoyo a hogares y pymes, condonación de pago de servicios
e impuestos, plan de rescate para comercio minorista y restaurantes, así
como información sobre si los gobiernos locales han solicitado más
recursos a la federación o se han endeudado para cubrir los gastos
extraordinarios causados por la pandemia e incluso contiene una pregunta
para identificar si se ha realizado un llamamiento de empresarios a no
pagar impuestos a la federación

La presente nota metodológica busca explicar cómo se construyeron los
indicadores a través de un análisis factorial de reducción de datos.
Primero se explica brevemente la técnica de análisis factorial y las
pruebas previas y después se presentan los principales resultados
estadísticos por apartado.

**Análisis factorial**

Este análisis busca reducir la dimensionalidad de un conjunto de
variables *x = \[x1, x2…Xn\]* correlacionadas entre sí en pocos factores
*Z = \[Z1, Z2…Zn\]* a partir de la combinación lineal de las variables
originales. Puntualmente lo que esta técnica permite es identificar qué
tanto de las variables originales pueden ser explicadas por factores
comunes y específicos como se indica en la siguiente ecuación:

![Formula](https://github.com/mexicovid/MexiCovidResearch/blob/master/Media/19_indicadores/image1.png?raw=true)

Donde Ξ sub c donde c = 1,2, …, c es el factor común que influye en la
variación de todas las variables y delta es el factor específico que
solamente afecta a la variable explicativa xi=1,2,…,n. Con este método
no solo se resume la información, sino además se permite jerarquizar las
variables según la importancia o correlación con cada factor la cual se
visualiza en una matriz de cargas factoriales rotada, el método de
rotación que aquí se empleó fue el de rotación Varimax. Finalmente, los
factores extraídos son los que pueden ser usados en lugar de los
variables originales y tienen la característica de que estos factores ya
no están están correlacionados entre sí.

El procedimiento para hacer el análisis factorial fue el siguiente: 1)
obtención de matriz de correlación de variables originales para
verificar que estuvieran correlacionadas entre sí, 2) realización de
pruebas previas al análisis factorial, 3) Correr el modelo de análisis
factorial para obtener la matriz de cargas factoriales y rotarla con el
método de rotación Varimax y 4) Obtención de los puntajes de las cargas
factoriales que representan la posición de las observaciones en el
espacio factorial, de la normalización de estos puntajes se obtuvieron
los 14 indicadores que resumen gran parte de la información contenida en
las 79 variables originales.

**Contrastes previos a la extracción de factores para evaluar la
pertinencia de la aplicación del análisis factorial**

Para evaluar si es posible hacer análisis factorial se realizan tres
pruebas. La primera consiste en identificar si el determinante de una
matriz de correlación se acerca a cero se garantiza que las
correlaciones entre las variables son muy altas. La segunda, es la de
esfericidad de Barlett cuya hipótesis nula es la existencia de una
matriz identidad (no correlación entre variables) y la tercera prueba es
la medida de Kaiser, Meyer y Olkin la cual sugiere que para valores
mayores que 0.5 y cercanos a 1 los datos son adecuados para hacer
análisis factorial.

En el Cuadro 1 se muestran las tres pruebas para cada sección
cuestionario y se observa que en cada una de ellas se cumplen al menos
dos de las tres pruebas para hacer el análisis factorial.

**Cuadro 1. Pruebas previas al análisis factorial**

<table>
<thead>
<tr class="header">
<th></th>
<th><strong>Sección</strong></th>
<th><strong>Pruebas</strong></th>
<th></th>
<th></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td></td>
<td></td>
<td><strong>Determinante de matriz de correlación</strong></td>
<td><p><strong>Contraste de esfericidad de Barlett**</strong></p>
<p><strong>(H0: las variables no están correlacionadas)</strong></p></td>
<td><p><strong>Kaiser-Meyer-Olkin</strong></p>
<p><strong>(KMO)</strong></p></td>
</tr>
<tr class="even">
<td><strong>1.</strong></td>
<td>Medidas de aislamiento</td>
<td>0.064</td>
<td><p>Chi-square= 71.76</p>
<p>p-value= 0.293</p></td>
<td>0.490</td>
</tr>
<tr class="odd">
<td><em><strong>1b.</strong></em></td>
<td>Medidas de aislamiento</td>
<td>0.239</td>
<td><p>Chi-square= 40.35</p>
<p>p-value= 0.000</p></td>
<td>0.689</td>
</tr>
<tr class="even">
<td><strong>2.</strong></td>
<td>Seguridad</td>
<td>0.123</td>
<td><p>Chi-square= 56.29</p>
<p>p-value= 0.121</p></td>
<td>0.499</td>
</tr>
<tr class="odd">
<td><strong>3.</strong></td>
<td>Trasparencia y comunicación</td>
<td>0.012</td>
<td><p>Chi-square= 117.93</p>
<p>p-value= 0.000</p></td>
<td>0.582</td>
</tr>
<tr class="even">
<td><strong>4.</strong></td>
<td><strong>Salud Pública</strong></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td></td>
<td>(Apartado a)</td>
<td>0.004</td>
<td><p>Chi-square= 143.96</p>
<p>p-value= 0.000</p></td>
<td>0.740</td>
</tr>
<tr class="even">
<td></td>
<td>(Apartado b)</td>
<td>0.054</td>
<td><p>Chi-square= 75.27</p>
<p>p-value= 0.566</p></td>
<td>0.506</td>
</tr>
<tr class="odd">
<td><strong>5.</strong></td>
<td>Economía</td>
<td>0.013</td>
<td><p>Chi-square= 111.263</p>
<p>p-value= 0.073</p></td>
<td>0.459</td>
</tr>
</tbody>
</table>

**Resultados estadísticos**

El criterio de reducción implica conservar aquéllos factores cuyos
valores propios son mayores a uno y que son capaces de explicar gran
parte de la varianza común. En el Cuadro 2 vemos que con los nuevos
factores se explica al menos 70% de la varianza y se sintetizó la
información contenida en 79 variables a únicamente 14 factores o
indicadores.

En la sección de aislamiento se pasó de 12 variables a 2 factores que
explican 74.23% de la varianza, en aislamiento 1b. se redujo la
dimensionalidad de 6 variables a 1 factor explicando el 95.61%, en
seguridad la reducción fue de 10 a 2 conservando 96.02% de varianza, en
Transparencia y comunicación se pasó de 11 variables a 2 factores que
explican 78.20% varianza, en salud pública de 26 variables originales a
4 nuevas variables que explican 87.49 y 72.50 % de la varianza para el
apartado a y el apartado b, respectivamente y, en economía la reducción
14 variables originales a 4 factores conservando el 82.48 % de la
varianza común.

**Cuadro 2. Factores extraídos y varianza explicada**

|           | **Dimensión**               | **Variables incluidas en el AF** | **Factores extraídos** | **Varianza acumulada explicada** |
| --------- | --------------------------- | -------------------------------- | ---------------------- | -------------------------------- |
| **1.**    | Aislamiento                 | 12                               | 2                      | 74.23%                           |
| ***1b.*** | aislamiento.                | 6                                | 1                      | 95.61%                           |
| **2.**    | Seguridad                   | 10                               | 2                      | 96.02%                           |
| **3.**    | Trasparencia y comunicación | 11                               | 2                      | 78.20%                           |
| **4.**    | **Salud Pública**           |                                  |                        |                                  |
|           | (Apartado a)                | 13                               | 2                      | 87.49%                           |
|           | (Apartado b)                | 13                               | 2                      | 72.50%                           |
| **5.**    | Economía                    | 14                               | 3                      | 82.48%                           |
|           | **Total**                   | **79**                           | **14**                 | **-**                            |

A continuación, se muestran las matrices rotadas de cargas factoriales
que representan la correlación entre las variables originales y el
factor extraído o, dicho de otra manera, indica la importancia o peso
relativo de la variable original en cada factor. Para interpretarse se
observan aquéllas que tengan una significancia estadística, la norma es
que cargas factoriales por arriba de 0.3 se consideran mínimas, por
encima de 0.4 son cargas importantes y por arriba de 0.5 son
significativas.

De la matriz de cargas factoriales sobre las medidas de aislamiento
(Cuadro 3) se observa en el factor 1 se cargan las variables que indican
cierre obligatorio de cafés y restaurantes, oficinas de servicios
profesionales, iglesias, cancelación de obras de construcción, cierre de
comercio bancos etc.; en el factor 2 solo se ve una correlación
significativa con las variables de cierre obligatorio de oficinas
gubernamentales, ya seas estatales o municipales.

<table>
<thead>
<tr class="header">
<th><strong>Cuadro 3. Matriz de cargas factoriales sobre las Medidas de Aislamiento</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><table>
<thead>
<tr class="header">
<th></th>
<th>Variable</th>
<th>Factor1</th>
<th>Factor2</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td></td>
<td><strong>Cierre obligatorio de…</strong></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td><strong>1.</strong></td>
<td>cafés y restaurantes</td>
<td>0.3333</td>
<td> -</td>
</tr>
<tr class="odd">
<td><strong>2.</strong></td>
<td>oficinas gubernamentales estatales</td>
<td> </td>
<td>0.8425</td>
</tr>
<tr class="even">
<td><strong>3.</strong></td>
<td>lugares de culto (iglesias)</td>
<td>0.4082</td>
<td> -</td>
</tr>
<tr class="odd">
<td><strong>4.</strong></td>
<td>oficinas gubernamentales municipales de la capital estatal</td>
<td> </td>
<td>0.6115</td>
</tr>
<tr class="even">
<td><strong>5.</strong></td>
<td>cancelación de obras públicas de construcción</td>
<td>0.5934</td>
<td> -</td>
</tr>
<tr class="odd">
<td><strong>6.</strong></td>
<td>oficinas y servicios profesionales</td>
<td>0.4187</td>
<td> -</td>
</tr>
<tr class="even">
<td><strong>7.</strong></td>
<td>comercio mayorista (centros comerciales y tiendas departamentales)</td>
<td>0.442</td>
<td> -</td>
</tr>
<tr class="odd">
<td><strong>8.</strong></td>
<td>comercio minorista (tiendas y comercio)</td>
<td>0.1913</td>
<td> -</td>
</tr>
<tr class="even">
<td><strong>9.</strong></td>
<td>bancos</td>
<td>0.1611</td>
<td> -</td>
</tr>
<tr class="odd">
<td><strong>10.</strong></td>
<td>maquilas e industria de transformación</td>
<td>0.4459</td>
<td> -</td>
</tr>
<tr class="even">
<td><strong>11.</strong></td>
<td>cancelación de obras privadas de construcción</td>
<td>0.5491</td>
<td> -</td>
</tr>
<tr class="odd">
<td><strong>12.</strong></td>
<td>Hay un calendario para retomar labores en las maquiladoras (en caso de haber suspensión)</td>
<td>0.2511</td>
<td> -</td>
</tr>
</tbody>
</table></td>
</tr>
</tbody>
</table>

Alpha Chronbach= 0.6578

Con la obtención de los puntajes de cada factor en la sección de medidas
de aislamiento se obtuvieron dos indicadores:

1.  Paro de actividad económica y cierre de espacios públicos

2.  > Cierre obligatorio de oficinas gubernamentales

En cuanto a la matriz de medidas de aislamiento llevadas a cabo por la
ciudadanía u organizaciones del sector privado (Cuadro 4) se observa que
tan las seis variables se correlación con un único factor, las que
tienen mayor importancia son poblaciones que bloquean el acceso de
automóviles foráneos y revisión revisiones de carreteras de entrada y
salida a sus comunidades; así como paro de obras de construcción. De los
puntajes a partir de este Factor se construyó el indicador:

1.  Acciones de la sociedad para evitar la propagación de la pandemia

**Cuadro 4. Matriz de cargas factoriales sobre las Medidas de
Aislamiento incentivadas por la ciudadanía**

|        | **Variable**                                                                                                                  | **Factor1** |
| ------ | ----------------------------------------------------------------------------------------------------------------------------- | ----------- |
| **1.** | Algunas poblaciones, por su cuenta, realizan revisiones en carreteras de entrada y salida a sus comunidades                   | 0.6697      |
| **2.** | Algunas poblaciones, por su cuenta, bloquean el acceso a automóviles de fuera, como medida de protección a posibles contagios | 0.7168      |
| **3.** | Los bancos tomaron la iniciativa de cerrar algunas sucursales                                                                 | 0.4834      |
| **4.** | Ha habido un cierre de maquilas e industrias de transformación                                                                | 0.5091      |
| **5.** | Las obras de construcción han sido detenidas                                                                                  | 0.6136      |
| **6.** | Se está realizando sanitización profunda en mercados y/o centrales de abasto                                                  | 0.3166      |

Alpha Chronbach= 0.7207

La matriz de cargas factoriales de la sección de seguridad (Cuadro 5)
refleja que en el Factor 1 se agrupan variables de actos violentos como
agresiones personas diagnosticadas por COVID-19, violencia familiar, así
como multas por violar el confinamiento o agredir a personal de salud.
En el Factor 2 se concentran actos como saqueos en comercio y centros
comerciales, hostilidad contra personal de salud así como operativos y
patrullajes para evitar saqueos o invitar a las personas a regresar a
sus casas.

De estos dos factores se obtuvieron dos indicadores:

1.  Violencia interpersonal y sanciones a agresiones e incumplimiento de
    confinamiento

2.  Violencia en espacios públicos y acciones de gobierno para cuidar el
    orden

**Cuadro 5. Matriz de cargas factoriales sobre Seguridad**

|         | **Variable**                                                                                | **Factor1** | **Factor2** |
| ------- | ------------------------------------------------------------------------------------------- | ----------- | ----------- |
| **1.**  | Han ocurrido saqueos a comercios y centros comerciales en las últimas dos semanas           | \-          | \-0.2363    |
| **2.**  | Hay operativos policiales y patrullajes para alentar a las personas a regresar a sus casas  | \-          | 0.512       |
| **3.**  | Hay patrullajes para evitar concentraciones en espacios públicos (playas, parques, plazas)  | \-          | 0.6067      |
| **4.**  | Se han registrado eventos de hostilidad de ciudadanos hacia personal de salud               | \-          | 0.5581      |
| **5.**  | Hay patrullajes en tiendas y centros comerciales para evitar saqueos                        | \-          | 0.406       |
| **6.**  | Se ha reportado un aumento de los casos de violencia familiar                               | 0.5228      | \-          |
| **7.**  | Hay multas por violar las reglas de confinamiento en los hogares                            | 0.4338      | \-          |
| **8.**  | Se han establecido penas o multas a aquellos que agredan al personal de salud               | 0.6049      | \-          |
| **9.**  | Se están presentando agresiones o ataques a personal de seguridad en los hospitales         | 0.6216      | \-          |
| **10.** | Se están presentando agresiones, maltratos o amenazas a vecinos diagnosticados con covid-19 | 0.3567      | \-          |

Alpha Chronbach= 0.5871

En la matriz de cargas factoriales de Transparencia y Comunicación
(Cuadro 6) se observa que las variables cargadas, o más correlacionadas,
al Factor 1 son aquellas que sugieren estrategias propias de los estados
para monitorear la COVID-19 pero también las declaratorias de
gobernadores para criticas las políticas federales para combatir la
pandemia o bien críticas sobre las estrategias federales de equipamiento
a los hospitales. En el factor 2 se asocian variables que ilustran las
estrategias de comunicación por los gobiernos locales como conferencias
diarias, existencia de sitio web, publicación de cifras de fuentes
propias, etc. De las puntuaciones de estos dos factores se obtuvieron
los siguientes indicadores:

1.  Declaratorias de crítica hacia políticas federales y actos de
    corrupción

2.  Herramientas estatales de transparencia y comunicación sobre la
    evolución de la pandemia

**Cuadro 6. Matriz de cargas factoriales de Transparencia y
Comunicación**

|         | **Variable**                                                                                                                                         | **Factor1** | **Factor2** |
| ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- | ----------- |
| **1.**  | El estado dedica una conferencia de prensa diaria para actualizar las cifras de confirmados                                                          | -           | 0.3969      |
| **2.**  | El estado tiene un sitio web para reportar las cifras oficiales de covid-19                                                                          | -           | 0.3364      |
| **3.**  | El estado ha desarrollado una aplicación móvil para consultar número de casos de Covid                                                               | 0.7256      | \-          |
| **4.**  | El estado ha desarrollado una aplicación móvil para consulta de pacientes con síntomas del Covid-19                                                  | 0.7         | \-          |
| **5.**  | Hay una línea telefónica para consulta de síntomas del Covid-19                                                                                      | -           | \-0.2668    |
| **6.**  | El estado publica sus cifras de fuentes propias y no reporta las de la fuente federal                                                                | -           | 0.3453      |
| **7.**  | El estado reporta las cifras de contagios confirmadas con pruebas de laboratorios privados y no solamente de las estatales                           | 0.3371      | \-          |
| **8.**  | El gobernador ha emitido declaraciones públicas donde crítica a las políticas federales de salud respecto al número de pruebas de Covid-19           | 0.8446      | \-          |
| **9.**  | El gobernador ha emitido declaraciones públicas donde crítica las políticas federales de equipamiento de hospitales (ventiladores, cubrebocas, etc.) | 0.8511      | \-          |
| **10.** | Se han presentado actos de corrupción con respecto a compras de materiales o similares vinculados con la pandemia                                    | -           | \-0.6142    |
| **11.** | Se han publicado notas periodísticas locales sobre desconfianza desde el estado de las cifras oficiales del Gobierno Federal del covid-19            | 0.6334      | \-          |

Alpha Chronbach= 0.582

**Salud Pública**

La matriz de cargas factoriales del Apartado a de Salud Pública (Cuadro
7a) revela que en el Factor 1 se cargan las variables de la existencia
de notas que recalcan la falta de equipamiento en hospitales, de
respiradores, saturación de hospitales, falta de material como batas y
cubrebocas, falta de material en el IMSS e ISSSTE. En el factor 2 se
agrupan las variables que reflejan algún tipo de ayuda como donación de
equipo médico por parte de las universidades, hoteles que dan resguardo
a personal de la salud, proporción de línea telefónica para atención
psicológica y ayuda para adultos mayores.

Los dos indicadores que se obtienen de las puntuaciones de estos dos
factores son:

1.  Saturación de hospitales, falta de personal médico y equipamiento

2.  Acciones de apoyo a población vulnerable o personal médico afectados
    por la pandemia

**Cuadro 7a. Matriz de cargas factoriales de Salud Publica (a)**

|         | **Variable**                                                                                                                      | **Factor1** | **Factor2** |
| ------- | --------------------------------------------------------------------------------------------------------------------------------- | ----------- | ----------- |
| **1.**  | Existe una línea estatal de atención psicológica para estrés traumático por covid                                                 |             | 0.6203      |
| **2.**  | El estado otorga algún tipo de apoyo a adultos mayores (ejemplo: mandados o comparas para adultos mayores a su casa)              |             | 0.6223      |
| **3.**  | Hay hoteles otorgando servicio de resguardo y hospedaje para personal de salud                                                    |             | 0.6345      |
| **4.**  | Universidades u organizaciones civiles locales se han organizado para donar equipo médico                                         |             | 0.6495      |
| **5.**  | Notas periodísticas han destacado la saturación de los hospitales a cargo de la entidad federativa (servicios estatales de salud) | 0.6217      |             |
| **6.**  | Notas periodísticas han destacado la saturación de los hospitales a cargo de la federación (imss, isstee)                         | 0.6005      |             |
| **7.**  | Ha habido notas destacando la falta de respiradores en la entidad                                                                 | 0.7036      |             |
| **8.**  | Notas periodísticas han recalcado la falta de material como batas y cubrebocas                                                    | 0.5557      |             |
| **9.**  | Notas periodísticas han recalcado la falta de equipo especializado como respiradores y camas de cuidados intensivos               | 0.8505      |             |
| **10.** | Notas periodísticas han señalado la falta de personal médico para brindar atención durante la pandemia                            | 0.5739      |             |
| **11.** | Han publicado notas acerca de falta de material médico y equipamiento en hospitales federales (IMSS o ISSSTE )                    | 0.6647      |             |
| **12.** | Se han publicado notas periodística acerca de falta de material médico y equipamiento en hospitales estatales                     | 0.5885      |             |
| **13.** | Se han publicado notas periodística acerca de falta de material médico y equipamiento en hospitales estatales                     | 0.492       |             |

Alpha Chronbach= 0.8078

La matriz de cargas factoriales del segundo apartado (Cuadro 7b) revela
que también hay dos factores. En el primero se correlacionan variables
para solucionar problemas como la saturación, por ejemplo, se tiene
reconversión de superficies a hospitales, aplicación de pruebas,
llamadas telefónicas para rastrear personas contagiadas, donaciones de
plasma, colaboración entre hospitales públicos y privados, manejo de
albergues de migrantes, decreto de uso de cubrebocas, fondeo con
recursos públicos para hacer más pruebas o equipamiento de salud. En el
Factor 2 se agrupan las variables de asignación de recursos estatales
para comprar materiales y equipamiento, donaciones por empresarios y
selección de hospitales para atender 100% a pacientes por COVID-19.

De los puntajes se obtuvieron otros dos indicadores para esta sección de
salud pública que son:

1.  Estrategias del estado para la detección, gestión y prevención del
    coronavirus COVID-19

2.  Preparación de hospitales y provisión de recursos públicos y
    privados para hacer frente a la COVID-19

**Cuadro 7b. Matriz de cargas factoriales de Salud Publica (b)**

<table>
<thead>
<tr class="header">
<th></th>
<th><strong>Variable</strong></th>
<th><strong>Factor1</strong></th>
<th><strong>Factor2</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><strong>1.</strong></td>
<td><blockquote>
<p>Hay superficies reconvertidas a hospitales (e.g. hoteles, estacionamientos, centros de convenciones)</p>
</blockquote></td>
<td>0.4572</td>
<td> -</td>
</tr>
<tr class="even">
<td><strong>2.</strong></td>
<td><blockquote>
<p>El estado está aplicando pruebas masivas para detectar casos positivos de coronavirus-20. El estado está realizando llamadas telefónicas a los hogares para detectar casos sospechosos de coronavirus-19</p>
</blockquote></td>
<td>0.4708</td>
<td> -</td>
</tr>
<tr class="odd">
<td><strong>3.</strong></td>
<td><blockquote>
<p>El estado está realizando llamadas telefónicas a los hogares para detectar casos sospechosos de coronavirus-19</p>
</blockquote></td>
<td>0.6386</td>
<td> -</td>
</tr>
<tr class="even">
<td><strong>4.</strong></td>
<td><blockquote>
<p>Se están haciendo donaciones de plasma de pacientes recuperados para el desarrollo de terapias de curación del coronavirus (covid-19)</p>
</blockquote></td>
<td>0.2742</td>
<td> -</td>
</tr>
<tr class="odd">
<td><strong>5.</strong></td>
<td><blockquote>
<p>El gobierno del estado tiene una iniciativa para que hospitales privados y públicos colaboren</p>
</blockquote></td>
<td>0.1598</td>
<td> -</td>
</tr>
<tr class="even">
<td><strong>6.</strong></td>
<td><blockquote>
<p>Hay un plan para regular la presencia de migrantes en albergues</p>
</blockquote></td>
<td>0.2885</td>
<td> -</td>
</tr>
<tr class="odd">
<td><strong>7.</strong></td>
<td><blockquote>
<p>El uso de cubreboca se ha decretado como una medida obligatoria en la calle</p>
</blockquote></td>
<td>0.3599</td>
<td> -</td>
</tr>
<tr class="even">
<td><strong>8.</strong></td>
<td><blockquote>
<p>El estado ha destinado recursos para compra de pruebas de covid-19</p>
</blockquote></td>
<td>0.6662</td>
<td> -</td>
</tr>
<tr class="odd">
<td><strong>9.</strong></td>
<td><blockquote>
<p>Ha llegado material de protección individual y equipamiento de salud del Gobierno Federal al estado</p>
</blockquote></td>
<td>0.227</td>
<td> -</td>
</tr>
<tr class="even">
<td><strong>10.</strong></td>
<td><blockquote>
<p>El estado ha destinado recursos para compra de material y equipo médico</p>
</blockquote></td>
<td> -</td>
<td>0.1218</td>
</tr>
<tr class="odd">
<td><strong>11.</strong></td>
<td><blockquote>
<p>Grupos de empresarios han donado material hospitalario (cámaras de comercio, clubes rotariales, etc)</p>
</blockquote></td>
<td> -</td>
<td>0.7084</td>
</tr>
<tr class="even">
<td><strong>12.</strong></td>
<td><blockquote>
<p>El estado ha seleccionado una serie de hospitales públicos donde se concentraran los casos con covid-19</p>
</blockquote></td>
<td> -</td>
<td>0.4751</td>
</tr>
<tr class="odd">
<td><strong>13.</strong></td>
<td><blockquote>
<p>Se han habilitado hospitales que tienen el 100% de su capacidad dedicada a atender pacientes con Covid-19</p>
</blockquote></td>
<td> -</td>
<td>0.6924</td>
</tr>
</tbody>
</table>

Alpha Chronbach= 0.574

Finalmente, la matriz de cargas factoriales de la sección de economía
(Cuadro 8) indica que las variables de reducción de tarifas, condonación
de impuestos o pago de agua, así como apoyos directos a hogares que han
perdido su empleo se correlacionan más con el Factor 1, las variables de
adquisición de deuda por parte del estado para comprar material médico,
así como intensiones de los gobiernos locales para rescatar comercio y
restaurantes, brindar apoyos a gastos funerarios están más
correlacionadas con el Factor 2. En el Factor 3 se cargan variables
asociadas a la existencia de un plan de apoyo a hogares que no pueden
pagar la renta, solicitud de recursos a la federación, empresarios para
no pagar impuestos a la federación y agotamiento de recursos para apoyar
a pymes.

De las puntuaciones de estos tres factores se generan los siguientes
indicadores:

1.  Apoyos de los gobiernos locales a las familias para aminorar las
    afectaciones económicas

2.  Endeudamiento y apoyos económicos

3.  Conflictos presupuestales generados a partir de la pandemia

**Cuadro 8. Matriz de cargas factoriales de Economía**

|         | **Variable**                                                                                                                | **Factor1** | **Factor2** | **Factor3** |
| ------- | --------------------------------------------------------------------------------------------------------------------------- | ----------- | ----------- | ----------- |
| **1.**  | El gobierno del estado ha establecido un programa de apoyos directos a hogares que han perdido su empleo                    | 0.2247      | \-          | \-          |
| **2.**  | Hay un plan de apoyo a hogares que no puedan pagar la renta de su vivienda                                                  | \-          | \-          | 0.55        |
| **3.**  | Se ha reportado que los recursos de apoyo a pymes o apoyos directos se han agotado por la gran cantidad de aplicantes       | \-          | -           | 0.3909      |
| **4.**  | Los municipios de la capital del estado o ciudades principales han condonado el cobro del agua potable                      | 0.4874      | \-          | \-          |
| **5.**  | Los municipios de la capital del estado o ciudades principales han condonado el cobro del impuesto predial                  | 0.7751      | \-          | \-          |
| **6.**  | El gobierno del estado ha adquirido deuda para comprar material médico                                                      | \-          | 0.6355      | \-          |
| **7.**  | El gobierno del estado ha adquirido deuda para solventar gasto durante la crisis económica                                  | -           | 0.6248      | \-          |
| **8.**  | Hay un plan de rescate o ayuda al comercio minorista y restaurantes                                                         | \-          | 0.4834      | \-          |
| **9.**  | El gobernador o la gobernadora han realizado un llamado a la Federación para incrementar los recursos económicos al estado. | \-          | \-          | 0.6814      |
| **10.** | El gobierno reparte despensas a las familias más necesitadas con motivo del Covid-19                                        | 0.3599      | \-          | \-          |
| **11.** | Hay notas periodísticas acerca del aumento del desempleo y despidos masivos en el estado                                    | \-          | 0.4494      | \-          |
| **12.** | Se han reducido las tarifas o se han dado apoyos para el pago de luz                                                        | 0.8006      | \-          | \-          |
| **13.** | Se están dando apoyos para gastos funerarios                                                                                | \-          | 0.3431      | \-          |
| **14.** | Empresarios locales han hecho llamamientos a no pagar impuestos a la federación                                             | \-          | \-          | 0.7395      |

Alpha Chronbach= 0.5252

Los indicadores descritos en esta nota metodológica son la normalización
de las puntuaciones factoriales y toman valores entre cero y uno,
valores cercanos a uno representan una mayor intensidad del fenómeno,
mientras que valores cercanos a cero indican menor intensidad o incluso
ausencia. Usted puede consultar los resultados en la sección de
Seguimiento por Regiones.
