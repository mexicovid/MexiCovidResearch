# Una Exploración de los Reportes de Movilidad de Google

Por: Roberto Ponce López

La Compañía Google tiene una iniciativa de datos públicos para apoyar a
gobiernos y actores sociales en la toma de decisión frente al Covid19.
La base de datos tiene una semana de desfase y se da a conocer cada
viernes en el sitio <https://www.google.com/covid19/mobility/>

## Descripción de los Datos

Los datos pueden ser descargados y compartidos de manera libre. Se trata
de datos anonimizados de usuarios de Android a partir de sus visitas a
establecimientos dentro de las categorías definidas por Google Place. En
el caso de México, los reportes se dan a conocer por entidad federativa
y comenzaron en la segunda semana de febrero del 2020. La base de datos
reporta la caída y aumento de la actividad diariamente para cada entidad
federativa en comparación con un punto de referencia anterior a la
pandemia, respecto a los seis rubros siguientes: a) comercio minorista y
ocio, b) compras de comestibles y farmacias, c) transporte público, d)
trabajo, e) parques y espacio público, y f) actividad en casa. La base
de datos reporta un dato de medición para cada una de estas actividades
y para cada día desde febrero del 2020 por entidad federativa. El punto
de referencia o *baseline* para el comparativo es la mediana del valor
de un índice de actividad correspondiente al día de la semana calculado
con los datos del periodo del 3 de enero al 6 de febrero del 2020. Los
datos de México analizados en este texto incluyen 92 observaciones por
estado, una por cada día de la semana del 15 de febrero al 16 de mayo,
enfocando nuestro análisis en las actividades de comercio minorista y
ocio, compras de comestibles y farmacias, transporte público y actividad
laboral.

## Exploración a nivel nacional 

La primera exploración consiste en una evaluación de los patrones de
actividad en el transcurso de la pandemia, observando los datos de las
32 entidades federativas en conjunto. Con este motivo, se calculó un
promedio móvil con los índices de Google para reducir los picos por los
cambios de patrones de actividad en los fines de semana. La Ilustración
1 visualiza estos resultados.

![A close up of a logo Description automatically
generated](./media/image1.png)

Ilustración 1. Promedios móviles de 5 días para los valores de actividad
en las 32 entidades federativas.

El lector o lectora puede apreciar dos elementos importantes en la
Ilustración 1. Por un lado, el largo vertical de las líneas para un día
en específico denota varianza importante en la reducción de actividad de
compras. Se puede apreciar varianza importante por estado para compra de
comestibles, transporte público y trabajo. Sin embargo, la caída en
comercio minorista y ocio fue bastante homogénea a nivel nacional, sin
grandes diferencias por región. En las otras actividades, sí encontramos
varianza importante en la adopción del confinamiento y reducción de
actividades.

Por otro lado, a partir de la segunda semana de marzo, se observa el
mismo patrón a nivel nacional: la caída más abrupta se registró en el
transporte público, segundo en compras minoristas, tercero en el trabajo
y finalmente en comestibles. Es interesante observar que en todas las
entidades se siguió el mismo patrón: ante las medidas de confinamiento,
la población recortó en primer lugar sus visitas al transporte público,
luego a las compras, luego al trabajo y finalmente a la compra de
comestibles.

## El Complicado Tema del Transporte Público

Los hogares que tuvieron a mano transporte privado en lugar de público
lo eligieron por ser un medio más seguro en la pandemia (observamos
caídas entre el 60 y el 80% dependiendo la entidad federativa). El
transporte público tendrá una serie de retos importantes conforme
volvamos a la normalidad con la reapertura económica. En primer lugar,
es previsible que, ante los riesgos de rebrote, muchos hogares seguirán
prefiriendo el transporte privado sobre el público, incrementando el
tráfico vehicular en las calles. En segundo lugar, la caída en la
demanda de transporte tendrá consecuencias serias para los operadores,
adicionando presión política sobre los organismos reguladores del
transporte en los estados. La mayor parte del transporte público en
México es operada por concesionarios privados y la tarifa es regulada
por las entidades federativas. La estructura de costos de estos
operadores funciona con base en dicha tarifa y con una demanda esperada.
De esta forma, la caída en demanda agregará presiones económicas a los
concesionarios de transporte público.

Adicionalmente, la caída en demanda es deseable porque esperas unidades
que viajen a la mitad de capacidad para reducir las probabilidades de
contagios. La única solución viable económicamente sería otorgar un
subsidio a los operadores de transporte para que operen a la mitad de
capacidad y no reduzcan frecuencia de servicio ante la caída en la
demanda. Sin embargo, las arcas estatales no parecen tener margen para
soportar una medida de este tipo. Vienen tiempos complicados para el
transporte público operado por concesionarios privados.

A continuación, exploremos las caídas de actividad para las 32 entidades
federativas de manera independiente. La Ilustración 4 muestra el
comportamiento de la actividad respecto a la línea base de medición por
actividad para cada uno de los estados.

![A close up of text on a white background Description automatically
generated](./media/image2.png)

Ilustración 2. Promedios móviles de 5 días para los valores de
actividad.

El lector o lectora puede identificar importantes diferencias
regionales. Yucatán, Quintana Roo, Ciudad de México y Baja California
son las entidades con las caídas más abruptas de actividad como producto
del confinamiento. En la mayoría de los estados, se puede observar que
las caídas en transporte público fueron en la misma proporción que las
compras minoristas. Aguascalientes, Nayarit, Puebla y Quintana Roo son
casos donde la caída en comercio minorista fue menor que la caída en
transporte público. Hidalgo es un caso atípico, es el único estado que
registró una caída mayor en el comercio minorista que en el transporte
público. Es difícil encontrar una explicación del caso de Hidalgo
porque hay muchas posibles hipótesis, una de ellas la forma urbana y
organización territorial de Hidalgo aunado a una baja tasa de tenencia
de automóvil.

Respecto a la actividad laboral, todas las entidades federativas
redujeron actividad en los lugares de trabajo a finales de marzo,
tocando un mínimo a principios de abril. A partir de la primera semana
de abril, se observa un incremento paulatino de la actividad laboral. En
Quintana Roo no se observa este repunte en trabajos, quizás por la
perdida masiva de empleos (ya no hay trabajo al cual regresar),
recordemos que el IMSS reportó una perdida de 50 mil empleos nada más en
marzo en esta entidad.

Los estados con la menor reducción en actividad laboral durante la
pandemia han sido Jalisco, Michoacán, Querétaro y Durango. El Estado de
México es un caso particular porque se observa una reducción importante
en actividad laboral, comercio minorista y transporte, pero no en
compras de comestibles. En el Estado de México, las visitas para compra
de comestibles y farmacia cayeron en una menor proporción que en el
resto de las actividades, comparando con el resto de las entidades
federativas.

Al observar la evolución de las líneas de actividad en el tiempo, llama
la atención el repunte general en actividad. En todos los estados se ha
observado este repunte de actividad a partir del mínimo de principios de
abril. La excepción sería Tabasco, donde la actividad se mantiene en
mínimos. El caso de Tabasco es interesante porque es la entidad
federativa con la mayor incidencia de contagios por 100 mil habitantes
después de la Ciudad de México.

## Reducción de Dimensionalidad a las Fechas y Actividades

En el análisis a continuación seleccionamos seis fechas específicas para
explorar actividad: miércoles 25 de marzo y sábado 28 de marzo,
miércoles 22 de abril y sábado 25 de abril, miércoles 13 de mayo y
sábado 15 de mayo. La selección de las fechas obedece a tener una
representatividad de actividad en un día a mitad de semana y en un día
de fin de semana, en tres periodos clave de la pandemia. De esta forma,
se seleccionaron las 6 fechas y las mediciones de actividad en los 4
rubros en cada una de ellas, resultando en 24 mediciones para cada una
de las 32 entidades federativas. A las 24 variables, se aplicó la
técnica de componentes principales para reducir la dimensionalidad de
los datos. La Ilustración 3 muestra la correlación e las variables por
fecha para las 24 componentes.

![A close up of a piece of paper Description automatically
generated](./media/image3.png)

Ilustración 3. Correlación de componentes principales y las 24 variables
de actividad por fecha (rr= retail, gr=groceries, tr=transit,
wk=workplace).

La correlación indica que la primera componente, la cual explica el 65%
de la varianza, arrastra algo de casi todas las variables, excepto
aquéllas de actividad del 16 de mayo. La segunda componente explica el
10% de la varianza y captura un efecto de las variables de transporte
púbico y comercio minorista. La tercera componente captura
principalmente el efecto de la actividad de finales de marzo, cuando las
caídas aún no eran tan abruptas. Con la finalidad de profundizar este
análisis, seleccionamos las componentes con *Eigenvalues* mayores a 1,
que resultaron ser las primeras cinco.

## Tipología de Entidades Federativas por Medidas de Acatamiento de las Medidas de Confinamiento

Con esas primeras cinco componentes, se realizó un clustering de
*kmeans*. Se siguió el método del codo para concluir que el número
óptimo de grupos era de 6. La Ilustración 4 gráfica la distribución de
las entidades federativas de acuerdo con las dos primeras componentes y
los seis grupos resultantes. El gráfico es un aproximado al resultado
final, ya que el agrupamiento se realizó con las primeras cinco
componentes y no dos. Exploremos la composición de cada grupo de
estados.

![A close up of a map Description automatically
generated](./media/image4.png)

Ilustración 4. Distribución de las 32 Entidades Federativas en las dos
primeras componentes y por grupo resultante del kmeans clustering

Las dos primeras componentes explican el 75% de la varianza y al
agrupamiento refleja proximidad de los grupos en estas dos dimensiones.
A continuación, caracterizamos los 6 grupos.

***Grupo 1: Aguascalientes, Baja California, Chihuahua, Nuevo León y
Sonora.*** Estos cuatro estados tienen la particularidad que redujeron
actividad de compras minoristas y de trabajo de manera importante. El
recorte en los viajes en transporte público fue el más importante
después de las entidades en el grupo 6. Sin embargo, la reducción en
visitas a compras de comestibles fue de las menores que se registraron
en el país.

***Grupo 2: Campeche, Ciudad de México, Sonora y Tabasco.*** Estas
cuatro entidades federativas se encuentran entre las más cumplidas en
términos de aislamiento. La actividad tuvo una disminución importante.
Después de los estados del grupo 6, las entidades del grupo 2 fueron las
más cumplidoras de la sana distancia.

***Grupo 3: Chiapas, Guerrero, Nayarit, Oaxaca, Puebla y Querétaro.***
Este grupo comparativamente con el resto de las entidades federativas,
no redujeron con la misma magnitud su actividad de compras y trabajo
durante la pandemia. Son el grupo que menos reducción de actividad tuvo
después del grupo 4.

***Grupo 4: Guanajuato, Hidalgo, Michoacán, Morelos, Estado de México,
Tlaxcala y Veracruz.*** Este grupo de estados son los que menos
redujeron su actividad laboral y de compras minoristas en comparación
con el resto de las entidades federativas. Sí hubo una reducción de
actividad, pero a la saga del resto de las entidades federativas.

Los grupos 3 y 4 son muy similares. La diferencia entre ambos es que
comparativamente, los estados del grupo 4 redujeron ligeramente en menor
proporción su actividad que los del grupo 4. Otra diferencia
significativa entre ambos grupos es que aquellos del grupo 3 redujeron
de manera muy importante sus viajes en transporte público el 25 de marzo
al inicio de la pandemia, más que los del grupo 4, pero aquellos del
grupo 3 paulatinamente han ido retomando sus viajes en transporte.

***Grupo 5: Coahuila, Colima, Durango, Jalisco, San Luis Potosí,
Tamaulipas y Zacatecas.*** La reducción de actividades en estas
entidades se ubicó en el promedio a nivel nacional. El elemento
distintivo de estos estados es que las mediciones del 13 y 16 de mayo
registraron un repunte importante de la actividad respecto a lo
observado en abril y marzo. Estas siete entidades dieron signos en mayo
de comenzar a retomar todas sus actividades, de trabajo como de como de
ocio.

***Grupo 6: Quintana Roo, Baja California Sur y Yucatán.*** Estos tres
estados son los más cumplidores en el aislamiento. Los tres bajaron su
actividad de manera radical y con la mayor magnitud a nivel nacional.
Quintana Roo y Baja California fueron de los estados con mayores brotes
per cápita en el inicio de la pandemia. El caso de Yucatán llama la
atención porque es un estado con una tasa relativamente baja desde el
inicio, pero que ha cumplido de manera encomiable las medidas de
aislamiento.

## Conclusión

Los patrones de actividad indican que de manera homogénea las personas
disminuyeron sus viajes y salidas de casa en el siguiente orden
descendente de mayor a menor: transporte público, trabajo, compras
minoristas y compras de comestibles. El primer punto de actividad que
los hogares deciden sacrificar es el uso del transporte público,
posiblemente debido al nivel de riesgo a contagio que se percibe en su
uso. Esto plantea un enorme reto de planeación para la gestión del
transporte público y sus economías conforme regresemos a la normalidad y
ocurran rebrotes.

Asimismo, se identificaron varianzas regionales importantes en la
rigurosidad de las medidas de aislamiento adoptadas. Los estados mejor
cumplidores de las medidas han sido Yucatán, Quintana Roo y Baja
California Sur. Después, han sido Campeche, Ciudad de México, Tabasco y
Sonora. Llama la atención la conducta ejemplar observada en toda la
Península de Yucatán.

Los estados *defiers* que menos han respetado el aislamiento son
Guanajuato, Hidalgo, Michoacán, Morelos, Estado de México, Tlaxcala y
Veracruz. Chiapas, Guerrero, Nayarit, Oaxaca, Puebla y Querétaro tampoco
han sido ejemplares. Finalmente, Coahuila, Colima, Durango, Jalisco, San
Luis Potosí, Tamaulipas y Zacatecas llaman la atención porque eran
estados bastante cumplidores de las medidas, pero donde se percibe un
relajamiento de las mismas en la segunda quincena de mayo.
