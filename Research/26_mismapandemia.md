MISMA PANDEMIA, DISTINTOS ESCENARIOS

La importancia del análisis y recolección de datos para la toma de
decisiones

**Introducción**

La epidemia del COVID-19 ha estado presente en todo el país, sin
embargo, diversos factores como la ubicación geográfica, la
infraestructura de los sistemas de salud y la incidencia de la pobreza,
han influido como se ha presentado la pandemia en las entidades
federativas.

El propósito de este trabajo es analizar las distintas similitudes en
las tasas epidemiológicas que presentan las entidades de la república
frente al COVID-19. Esto con el objetivo de demostrar los distintos
escenarios que existen en el país y cómo estos han modificado el
comportamiento de los tomadores de decisiones.

Se realizó un comparativo de las tasas de letalidad, mortalidad,
positividad y un coeficiente diseñado para propósitos del análisis
llamado, Coeficiente C. De este comparativo se encontraron diferencias
regionales puntualizadas, debido a la diferencia en la incidencia de los
niveles de cada tasa dependiendo de distintos factores. A su vez también
se realizó una agrupación de las entidades mediante el método de K-Means
para tener un mejor entendimiento de la incidencia regional de las tasas
epidemiológicas.

Las tasas epidemiológicas son un gran instrumento para analizar los
distintos escenarios que presentan el país. Las tasas son el resultado
de la relación entre dos magnitudes como lo podría ser la cantidad de
población y la cantidad de pruebas realizadas. Esta relación es
proporcional a las dos magnitudes, por lo que son de gran utilidad al
comparar distintas regiones o entidades.

Estas tasas nos permiten conocer, en un contexto general, la situación
que presenta cierta región. Al momento de analizarlas se puede obtener
con más certeza la efectividad de las políticas públicas o medidas de
movilidad para reducir la propagación o letalidad del virus. Con esta
certeza otorgada se puede tener una respuesta más de acuerdo con la
situación que se presenta y no depender de supuestos.

La situación de México no se ha visto favorable en comparación con otros
países. De acuerdo con TResearch (2020), consultora número 1 en asuntos
públicos online, México se encuentra en el 6º lugar de más contagios
globales y 4º lugar de más muertes absolutas y por día. El país también
se encuentra en el número 20 de pruebas realizadas por cada 100 mil
habitantes en América.

**Metodología**

Para la realización de este análisis utilizamos la base de datos al día
21 de Julio del 2020 proporcionada por la Secretaría de Salud del
gobierno de México en su página de Datos Abiertos, así como la base de
datos de población proporcionada por el Instituto Nacional de
Estadística y Geografía al 2020.

En la base de datos de la Secretaría de Salud se pueden observar las más
de 840 mil pruebas de COVID acumuladas desde inicios de la pandemia,
tanto positivas como negativas y en proceso, en cada prueba se describe
el caso del paciente y las características que presenta como edad,
unidad médica donde fue atendido, comorbilidades, resultado de la
prueba, fecha de defunción, fecha de ingreso, entre otras.

Utilizamos el lenguaje de programación Python para trabajar sobre la
base de datos proporcionada, donde a su vez generamos unas nuevas
variables que posteriormente subimos a Tableau con el fin de tener una
representación más limpia y estable de los resultados. Para realizar
nuestro análisis hicimos el cálculo de las variables de tasa de
positividad, tasa de mortalidad y tasa de letalidad, así como también el
diseño del Coeficiente C.

La tasa de letalidad es la cantidad de fallecidos por COVID-19 sobre la
cantidad total de positivos, es decir la probabilidad de fallecimiento
en caso de contraer el virus.

Tasa de letalidad =
\(\frac{Cantidad\ de\ Fallecimientos\ por\ COVID - 19}{\text{Cantidad\ de\ Positivos\ }}\ x\ 100\)

La tasa de mortalidad es la proporción de personas que fallecieron de
COVID-19 por cada 100 mil habitantes del estado o región, esta tasa nos
indica el impacto real que tienen los fallecimientos con respecto al
tamaño del estado. Su fórmula es:

Tasa de mortalidad =
\(\frac{Cantidad\ de\ Fallecimientos\ por\ COVID - 19}{Cada\ 100\ mil\ hab\ }\)

La tasa de positividad es la cantidad de casos confirmados respecto a la
cantidad de pruebas realizadas, es decir la probabilidad de que una
persona salga positivo de COVID-19.

Tasa de positividad =
\(\frac{\text{Cantidad\ de\ Pruebas\ Positivas}}{\text{Cantidad\ de\ Pruebas}}\ x\ 100\)

El Coeficiente C fue diseñado con el objetivo de relacionar la cantidad
de pruebas de un Estado o Región con respecto a la cantidad de
población. El coeficiente C evalúa la cantidad de pruebas con respecto
al 10% de la población de la región, esto con el objetivo que el estado
o país que realice la misma cantidad de pruebas que una décima parte de
su población tenga un coeficiente de 1.

Se decidió utilizar el 10% de la población ya que los países que han
presentado una tasa de positividad menor al 5% han realizado un
aproximado de 100 pruebas por cada 1,000 habitantes. Al calcular la
relación en cuanto a la raíz cuadrada de ambas cifras se obtiene una
mejor comprensión de la magnitud del coeficiente, ya que resulta en una
escala más entendible.

Este coeficiente nos permite evaluar los esfuerzos que está realizando
cada estado para tener un mayor control sobre las cifras de la pandemia
y así realizar decisiones más acertadas.

Coeficiente C =
\(\frac{\sqrt{\text{Cantidad\ de\ las\ pruebas\ }}}{\sqrt{10\%\ de\ la\ población\ }}\)

**Comparativo entre Estados**

Para poder analizar e identificar las similitudes entre los 32 estados
de una manera más amigable con la audiencia, utilizamos el Método de
Agrupamiento de K-Means, se emplearon las 4 variables descritas
anteriormente: tasa de letalidad, tasa de mortalidad, tasa de
positividad y el Coeficiente C.

El uso de las tasas epidemiológicas nos da un mejor contexto al momento
de analizar las variables en distintas entidades. Nos otorgan un mejor
entendimiento sobre las acciones que han tomado los gobiernos de los
estados.

Al agrupar a los estados podemos observar que muchos de estos han
mantenido una misma o similar línea de acción. La similitud entre los
planes de acción de los estados es el resultado del conjunto de
distintos factores, entre los que destacan los factores geográficos,
sociales y económicos.

El resultado obtenido fue 5 grupos, los cuales describiremos a
continuación, así como el resultado de cada variable. Es importante
notar que las comparaciones se hacen dentro de estos mismos grupos por
lo que una baja tasa no significa que en realidad sea baja, sino que a
comparación con los otros lo es. En la figura 1 podemos observar los
estados que conforman cada grupo, así como el resultado de cada
variable.

![](./media/image1.png)

*Figura 1. Gráfica del Comparativo entre estados*

**Grupo 1.**

Los estados pertenecientes a este grupo se caracterizan por tener una
**tasa de letalidad** y **tasa de mortalidad** baja, la población y el
gobierno han podido reducir el impacto en cuestión de vidas humanas con
políticas de distanciamiento social y una mejor comunicación entre ambos
entes. Las probabilidades de fallecer a causa del COVID-19 son menores a
comparación de otros estados y la cantidad de muertes en relación a la
población de las entidades es menor a comparación de otras en el país.

La **tasa de positividad** es baja y cuentan con un **Coeficiente C**
medio, demostrando el trabajo de realizar la cantidad de pruebas
considerable en proporción a su población. Gracias a esto han podido
cuantificar con mayor exactitud la cantidad de casos confirmados.
Geográficamente estos estados están ubicados en las zonas Norte y
Centro del país.

Las acciones tomadas por los gobernadores de este grupo han tenido una
respuesta positiva en favor del manejo de la propagación del virus,
logrando un promedio de tasas favorables en comparación al resto del
país. Cabe destacar que la mayoría de los gobernadores de los estados
de este grupo se declararon en desacuerdo con el plan federal del
Semáforo Epidemiológico.

En este grupo encontramos a los estados de Tamaulipas, Nuevo León y
Coahuila los principales actores, debido a la actividad económica. En la
*Figura 2* podemos observar a mayor detalle las estadísticas del grupo
1.

![](./media/image2.png)

Figura 2. Gráfica del Grupo 1

**Grupo 2.** Tiene como principales características una alta **tasa de
letalidad** y una baja **tasa de mortalidad**, que representa una baja
cantidad de fallecimientos con respecto a la población, pero una
probabilidad muy alta de fallecer en caso de contraer el virus. En estos
estados esto podría influir en el comportamiento de la población al
representar un mayor riesgo, agudizando aún más las medidas en
comparación de otras entidades.

También cuentan con una alta **tasa de positividad** y un bajo
**Coeficiente C**, que tiene como significado una baja cantidad de
pruebas en proporción a su población y una alta probabilidad de obtener
un resultado positivo por prueba realizada. Debido a los niveles de
ambas variables se tiene un alto grado de incertidumbre con respecto a
las cantidades reales de confirmados y de fallecimientos.

Un descuido en la medición de los casos reales podría significar un
aumento imprevisto muy importante en la tasa de mortalidad en el corto y
mediano plazo, debido a que existe incertidumbre en la cantidad de casos
reales y la gravedad de estos.

Geográficamente estos estados están ubicados en las zonas del centro y
sureste del país.

En la *Figura 3* podemos observar a mayor detalle las estadísticas del
grupo 2.

![](./media/image3.png)

Figura 3. Gráfica del Grupo 2

**Grupo 3**. Este grupo comparte ciertas similitudes con el grupo 2 en
las tasas de positividad y letalidad, sin embargo, sus diferencias en la
tasa de mortalidad y el coeficiente C pueden significar escenarios
sucesivos.

La **tasa de positividad** es alta pero el **Coeficiente C** tiene un
nivel medio, estas variables podrían significar un esfuerzo ligeramente
mayor en realizar pruebas. A pesar de esto no parecen ser suficientes
para medir la cantidad real de casos. El grado de incertidumbre es muy
alto, debido a que las tasas de positividad oscilan entre el 60 y 50 %.

Los estados presentan una **tasa letalidad** alta, así como también una
**tasa de mortalidad** media. Como observamos el nivel de la tasa de
mortalidad es más alto que el grupo 2, ambos con altos niveles de
vacilación. La incertidumbre podría generar un crecimiento imprevisto de
la cantidad de fallecimientos y a su vez crear una mayor saturación en
los sistemas de salud.

Estos estados han podido reducir el impacto de los fallecimientos en su
población general con una tasa de mortalidad media, sin embargo, las
estrategias y planes de acción de gobierno y ciudadanía podrían ser
sesgados por la falta de información que presenta debido a que no se
realizan las pruebas necesarias.

Geográficamente estos estados están ubicados en las zonas del norte y
sureste del país.

En la *Figura 4* podemos observar a mayor detalle las estadísticas del
grupo 3.

![](./media/image4.png)

Figura 4. Gráfica del Grupo 3

**Grupo 4**. Este grupo está conformado por solamente dos estados y
presentan características diferentes a las demás entidades, que a su vez
forman escenarios distintos.

Los estados de este grupo presentan una **tasa de positividad** media y
un **coeficiente C** muy alto. Como se observa el grado de incertidumbre
proporcionado por la tasa de positividad se ha reducido al aumentar la
cantidad de pruebas. Esta estrategia pudo ser motivada debido a los
brotes constantes en diversas localidades de estas entidades.

En el apartado de fallecimientos, estos tienen unas tasas de
**letalidad** y **mortalidad** muy altas, estas representan la
probabilidad de fallecer en caso de contraer la enfermedad y el impacto
real en la población de las entidades. La condición de salud de la
población de estas entidades podría ser un factor importante para
evaluar las condiciones

Mediante un análisis a la base de datos de las pruebas de COVID-19,
proporcionada por la Secretaría de Salud, encontramos que la diabetes es
la segunda patología más común en las defunciones por COVID-19 con un
40% de incidencia.

En el 2018, un estudio analizó distintas dependencias del Instituto
Mexicano del Seguro Social (IMSS) y determinó a la Ciudad de México como
una de las etiquetadas donde mayor prevalencia de diabetes ha sido
informada (Ovalle-Luna, 2019). Por otro lado, Tabasco es la entidad con
mayor tasa de mortalidad por diabetes, siendo 10.6 muertes por cada 100
mil habitantes, según el informe de Características de Defunciones de la
INEGI.

Geográficamente estos estados están ubicados en la zona Centro del país.
En la *Figura 5* podemos observar a mayor detalle las estadísticas del
grupo 4.

![](./media/image5.png)

Figura 5. Gráfica del Grupo 4

**Grupo 5.** La característica que más destaca de este grupo es la baja
**tasa de mortalidad** .Por otro lado la **tasa de letalidad** es alta,
esto podría causar a mediano plazo que el aumento en los casos positivos
tenga una repercusión directa en la cantidad de fallecimientos
aumentaron, debido a las altas posibilidades de fallecer de los
ciudadanos.

El bajo **Coeficiente C** y la **tasa de positividad** en un nivel medio
nos indica una gran área de oportunidad en cuanto a la cantidad de
pruebas. La certidumbre que genera la tasa de positividad no es tan
crítica en comparación de otros estados, sin embargo, el Coeficiente C
tan bajo nos indica que no se están haciendo las pruebas suficientes
para la correcta monitorización de la enfermedad. A pesar de su tasa de
positividad se sigue sin tener una correcta medición de los casos,
presentando el riesgo de actuar a ciegas por parte del gobierno y
afectando aún más las actividades económicas de estos estados.

Geográficamente estos estados están ubicados en las zonas del norte y
centro del país.

En la *Figura 6* podemos observar a mayor detalle las estadísticas del
grupo 5.

![](./media/image6.png)

Figura 6. Gráfica del Grupo 5

El comportamiento de los 5 grupos de acuerdo con las cuatro variables
previamente analizadas se puede representar de una manera gráfica en la
F*igura 7*. Con esto podemos observar las diferencias que presenta cada
grupo y como es que tienen un comportamiento similar al interior de cada
grupo.

![](./media/image7.png)

Figura 7. Segmentación por grupos (KMeans)

**Comparativo internacional**

De acuerdo con la conferencia de prensa que dio la Organización Mundial
de la Salud, las tasas de positividad de los países que han hecho una
extensa cantidad de pruebas han oscilado entre el 3% y el 12%. La
principal razón de las distintas cantidades de pruebas entre países y
dentro de los mismos recaen en dos razones principales, los recursos de
cada región son distintos, así como el impacto de la epidemia ha sido en
mayor o menor medida a distintos sectores fundamentales de los países.

La dependencia de cada país a los sectores más afectados es distinta,
por lo que un país dependiente del sector turístico o el transporte
tendría un mayor impacto a sus actividades económicas, que un país
dependiente de un sector no tan afectado como lo podría ser el
E-Commerce.

La existencia de tasas de positividad muy altas como en Latinoamérica,
entre 60% - 80%, significa que no existe una monitorización de los casos
y la gravedad de estos correctamente. Esta falta de información ocasiona
un sesgo en la información, causando que las medidas para detener la
pandemia o reducir los efectos de esta no tengan resultados. No conocer
la información relevante de tus enfermos y la ubicación de estos
terminan en la pérdida de vidas humanas.

De acuerdo con los datos recuperados de Statistics, los dos países con
más pruebas son China y Estados Unidos, estos cuentan con una tasa de
positividad de 0.1% y 8% respectivamente, y con un Coeficiente C de 0.8
y 1.35. Las bajas tasas de positividad nos indican que se están haciendo
una gran cantidad de pruebas y nos ayuda a entender cómo es que la
pandemia está progresando con unas cifras más apegadas a la realidad. El
que el Coeficiente C esté elevado y las bajas tasas de positividad nos
indica como el Coeficiente C es una gran herramienta para evaluar la
cantidad de pruebas que se están haciendo son las ideales.

La situación de México es muy diferente como se mencionó anteriormente,
el país cuenta con una tasa de positividad de 43.7% y un Coeficiente C
de 0.23, en contraste con China y EUA, se tiene una alta tasa de
positividad y un Coeficiente C muy bajo. No se están haciendo las
suficientes pruebas por lo que muchos casos quedan sin ser monitoreados
y evaluados. El impacto que genera esta falta de información es directo:
la población y gobierno podrían orientar sus decisiones de una manera
incorrecta, así como también destinar recursos limitados a estrategias
ineficientes.

**Conclusión**

Los Estados tienen una enorme área de oportunidad en cuanto a cantidad
de pruebas se refiere. Esto ayuda a que se tengan datos más apegados a
la realidad y así poder analizar el desarrollo de la pandemia. Con esto
los gobiernos podrán tener una mejor perspectiva y así tomar decisiones
que tengan un impacto verdadero y analizar el desarrollo de este.

Como sabemos, la cantidad de recursos es limitada, es aquí donde entra
la importancia en saber dónde es más eficiente destinar estos recursos,
sobre todo ahora que tenemos una capacidad del sistema de salud tan
limitada. En la misma línea de eficientar los recursos se deben de tener
diferentes planes de acción para los estados ya que la pandemia no se
presenta de la misma manera en todas las entidades. De esta manera se
podría hacer un uso de recursos más específico a las condiciones que se
presentan, ya que se tendría más información sobre el desarrollo de la
pandemia y el impacto que tiene en la población. Al momento de
generalizar no estamos considerando todas las variables que terminan por
hacer un uso incorrecto de recursos económicos o humanos.

Se observa como el Coeficiente C puede ser un indicador eficiente para
evaluar la situación en el apartado de pruebas que enfrenta tanto el
país como los estados. Al complementarse con la tasa de positividad
podemos observar si están haciendo las pruebas suficientes y las áreas
de oportunidad que presentan. Analizando las dos variables en un
diagrama de dispersión, se observa que, entre mayor Coeficiente C, la
tasa de positividad es menor, demostrando una relación negativa y
justificando la utilidad del coeficiente.

Las tasas epidemiológicas han presentado los distintos escenarios que
existen en el país, así como distintas hipótesis sobre el porqué de las
situaciones. A pesar de existir muchos factores en la evaluación de un
estado o región, las tasas han sido de gran utilidad para concluir que
las situaciones son presentadas en distinta magnitud diferenciadas por
su regionalidad.

Todos los estados enfrentan la misma pandemia, pero no en igualdad de
condiciones. Los recursos han jugado un papel importante a su vez y
también los esfuerzos que ha hecho cada estado por recolectar
información en beneficio a su ciudadanía y a los planes de acción.

El país enfrenta un gran reto por delante, las tasas presentadas en un
comparativo estatal tienden a ser bajas o altas, sin embargo, en un
comparativo internacional México se encuentra en las situaciones más
críticas. La falta de información, la vulnerabilidad en la salud de la
población, la saturación hospitalaria del sistema público y la situación
económica del país, terminaron siendo los factores más determinantes del
país. El correcto uso de la tecnología para facilitar la recolección y
análisis de datos, así como el aumento en la cantidad de pruebas serían
los primeros pasos para una verdadera nueva normalidad.

**Referencias**

Gobierno de México. (2020, Julio 21). Datos Abiertos - Dirección General
de Epidemiología. Recuperado de:
[<span class="underline">https://www.gob.mx/salud/documentos/datos-abiertos-152127</span>](https://www.gob.mx/salud/documentos/datos-abiertos-152127)

INEGI (2019, octubre 31). Características de las defunciones registradas
en México durante 2018. Disponible en:

[<span class="underline">https://www.inegi.org.mx/contenidos/saladeprensa/boletines/2019/EstSociodemo/DefuncionesRegistradas2019.pdf</span>](https://www.inegi.org.mx/contenidos/saladeprensa/boletines/2019/EstSociodemo/DefuncionesRegistradas2019.pdf)

Our World Data. (2020, Agosto 4). Coronavirus (COVID-19) Testing -
Statistics and Research. Recuperado de:
[<span class="underline">https://ourworldindata.org/coronavirus-testing</span>](https://ourworldindata.org/coronavirus-testing)

Ovalle-Luna, O. D., Jiménez-Martínez, I. A., Rascón-Pacheco, R. A.,
Gómez-Díaz, R. A., Valdez-González, A. L., Gamiochipi-Cano, M., ... &
Sánchez-Becerra, M. C. (2019). Prevalencia de complicaciones de la
diabetes y comorbilidades asociadas en medicina familiar del Instituto
Mexicano del Seguro Social. *Gaceta medica de México*, *155*(1), 30-38.
[<span class="underline">https://www.medigraphic.com/cgi-bin/new/resumenI.cgi?IDARTICULO=85632</span>](https://www.medigraphic.com/cgi-bin/new/resumenI.cgi?IDARTICULO=85632)

Statista. (2020, Agosto 3). Coronavirus cases worldwide by country.
Recuperado de:
[<span class="underline">https://www.statista.com/statistics/1043366/novel-coronavirus-2019ncov-cases-worldwide-by-country/</span>](https://www.statista.com/statistics/1043366/novel-coronavirus-2019ncov-cases-worldwide-by-country/)

Statista. (2020, Agosto 3). COVID-19 test by country. Recuperado de:

[<span class="underline">https://www.statista.com/statistics/1028731/covid19-tests-select-countries-worldwide/</span>](https://www.statista.com/statistics/1028731/covid19-tests-select-countries-worldwide/)

WHO? (2020, Marzo 30). COVID-19 - virtual press conference. Disponible
en

[<span class="underline">https://www.who.int/docs/default-source/coronaviruse/transcripts/who-audio-emergencies-coronavirus-press-conference-full-30mar2020.pdf?sfvrsn=6b68bc4a\_2</span>](https://www.who.int/docs/default-source/coronaviruse/transcripts/who-audio-emergencies-coronavirus-press-conference-full-30mar2020.pdf?sfvrsn=6b68bc4a_2)

**Anexos**

**Anexo 1. Distribución geográfica por Grupo**

![](./media/image8.png)
