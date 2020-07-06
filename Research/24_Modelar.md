Modelar lo impredecible: lecciones sobre el desarrollo de herramientas
de apoyo a la toma de decisiones para COVID19 en México

¿Cuándo terminará el brote de COVID19? ¿Hemos aplanado la curva? ¿Cuándo
es seguro reabrir la economía? Estas son preguntas que están en la mente
de todos en México y que han suscitado un acalorado debate en el país.
Para responder de manera útil, necesitamos producir análisis
fundamentalmente diferente al que estamos acostumbrados.

Esta nota resume el trabajo que algunos colegas y yo en el Tecnológico
de Monterrey hemos llevado a cabo para desarrollar un modelo de
simulación de COVID19 en México. El propósito de este modelo es ayudar
a las autoridades estatales y al público a entender cómo está
progresando la pandemia en su región, simular trayectorias plausibles
del virus en el corto plazo y estudiar con mayor detalle los riesgos de
reabrir la economía en este momento. Durante el desarrollo de este
modelo hemos interactuado con una amplia gama de talentosos analistas y
tomadores de decisiones, lo cual nos han llevado a generar importantes
lecciones que vale la pena compartir.

Cualquier brote pandémico es incierto. Sin embargo, en el caso de
COVID19, la incertidumbre epidemiológica inherente al virus es
exacerbada por la naturaleza impredecible del comportamiento humano, las
dificultades de explicar información compleja al público y por debates
políticos. Intentar mantenerse al día con la pandemia es uno de los
desafíos analíticos más grandes que hemos enfrentado.

Nuestro modelo (EgobiernoyTP-SIR) es un modelo SIR clásico, ampliado
para describir la dinámica de cinco grupos poblacionales: 1)
susceptibles, 2) infectados, 3) recuperados, 4) hospitalizados y 5)
fallecidos. El modelo tiene dos características importantes: 1) está
diseñado para modelar una amplia gama de opciones de contención (e.g.,
distanciamiento social, rastreo de contactos, aislamiento, pruebas y
vacunación), y 2) la suposición base del modelo es tratar al número
oficial de casos confirmados y población fallecida como información
retrasada sobre la evolución real de la pandemia. Es posible obtener más
información sobre el modelo visitando:
[<span class="underline">https://mexicovid19.app/simulatio</span>](https://mexicovid19.app/simulatio)
y el repositorio GitHub en donde reside una versión pública del modelo:
<https://github.com/emolinaperez/Covid_MX> .

Los supuestos descritos anteriormente suenan razonables. Sin embargo,
¿nuestro modelo es perfecto? NO, NO LO ES. Ningún modelo lo es. Los
modelos de simulación son perfectibles y siempre se pueden mejorar. El
nuestro en particular puede mejorarse desagregando las cohortes de
población y pacientes hospitalizados, aumentando la granularidad de las
intervenciones políticas consideradas (e.g., considerando el impacto
marginal del uso de tapabocas) y modelando los retrasos de información
como dinámicos. Áreas en las que estamos trabajando en este momento.

Lo anterior no impide que el modelo sea útil como herramienta de apoyo a
la toma de decisiones. En mi opinión, para poder desarrollar
herramientas de apoyo a la toma de decisiones que sean útiles y
eficaces, el primer paso es poner a prueba el modelo contra el registro
histórico. Si un modelo de simulación no es capaz de replicar
razonablemente las condiciones históricas, es muy difícil confiar en el
análisis derivado del modelo. Calibrar el modelo de una manera rigurosa
ayuda a mejorarlo, entender sus limitaciones y aumentar la confianza en
su desempeño.

Dada la importancia y sensibilidad pública de COVID19, elegimos poner a
prueba nuestro modelo con datos sobre casos y muertes confirmadas en los
32 estados de México. Hicimos esto para asegurarnos de que el modelo sea
capaz de producir una descripción plausible de cómo está progresando la
pandemia en México. Esta no es una hazaña trivial, replicar ambos
registros a nivel regional significa que nuestra descripción matemática
de la pandemia (i.e., sistema de ecuaciones diferenciales) necesita
ajustarse a ambos conjuntos de datos, y así proporcionar una descripción
armonizada de lo que está sucediendo en cada región.

El siguiente gráfico muestra un ejemplo de este ejercicio. Compara el
comportamiento de nuestro modelo (líneas naranjas) con el número
histórico de casos confirmados y muertes (líneas azules) en la Ciudad
de México. En este caso es posible ver que nuestro modelo es capaz de
replicar razonablemente el comportamiento histórico de la pandemia en
esta región. Una vez que encontramos la combinación de parámetros que es
capaz de hacer esto, etiquetamos esta combinación paramétrica como
"condición de línea de base". Conseguir que el modelo pueda hacer esto
para 32 estados requirió muchas, muchas ... muchas noches de escribir
código. En última instancia, logramos esto expandiendo y mejorando la
estructura matemática del modelo varias veces, utilizando registros de
datos de movilidad de dispositivos celulares, e implementando una
versión multivariada del método de máxima verosimilitud (MLE) con los
criterios de descomposición de Theil, y aún no hemos terminado, ya que
este proceso de calibración está constantemente ilustrando nuevas
maneras en las que podemos mejorar nuestro trabajo.

![](./media/image1.png)

Esta característica del modelo no significa que el modelo sea perfecto,
o que se pueda utilizar como una bola de cristal para predecir lo que va
a pasar con la pandemia en el futuro. Cumplir con este umbral mínimo de
calidad, significa fundamentalmente que el modelo se puede utilizar como
laboratorio para la experimentación (i.e., es parcialmente válido).
Después de esto, muchas mejoras se derivan de socializar los resultados
con expertos y actores interesados, cuya crítica nos ha ayudado a
resolver deficiencias en nuestro trabajo. La combinación de ambos
procesos: calibración estadística rigurosa y retroalimentación crítica
nos ha ayudado a mejorar sustancialmente el modelo.

Las lecciones derivadas de experimentar con el modelo son
particularmente útiles para entender dónde estamos en la pandemia, cómo
llegamos aquí y cuáles son las disyuntivas críticas hacia adelante. No
puedo subrayar este punto lo suficiente, especialmente para el caso de
COVID19. La progresión de la pandemia es lo suficiente compleja y
volátil que cualquier esfuerzo de predicción está destinado al fracaso.
A pesar de esto, todos los días vemos en nuestras cuentas de twitter y
periódicos profecías constantes sobre COVID19. En los peores casos,
escuchamos a funcionarios públicos publicitar días exactos en los que se
terminará la pandemia. Desde mi punto de vista, esto crea ansiedad entre
el público y los tomadores de decisiones, y frustración cuando estas
profecías no se cumplen.

El modelo descrito en los párrafos anteriores tiene varias aplicaciones.
La primera es que se puede utilizar para estimar rangos de valores del
número real de casos confirmados y la población fallecida (i.e.,
empleando bootstrapping). En la figura siguiente, la línea azul muestra
el registro histórico de los casos confirmados (panel izquierdo) y la
población fallecida (panel derecho). Las líneas naranjas y los diagramas
de caja describen el rango de valores para la estimación de valores
reales de ambas variables.

![](./media/image2.png)

No debería sorprendernos que exista una diferencia entre el registro
histórico y los valores reales estimados. El valor de este ejercicio
reside en el hecho de que podemos estimar un rango de valores para ambas
cifras con cierto grado de rigor estadístico. En este ejemplo, para la
Ciudad de México, de acuerdo a nuestra estimación, el 7 de junio, el
número real estimado de casos osciló entre 151 y 234 mil individuos,
esto es aproximadamente cinco veces mayor que el registro histórico.
Para la población fallecida, el valor real estimado oscilaba entre 13 y
21 mil muertes, esto es cuatro veces mayor que el registro histórico
–testimonio del gran costo humano de COVID19-. Hay algunos matices de
estos rangos sobre los que vale la pena ahondar.

¿Pueden cambiar estas estimaciones? Absolutamente, a medida que se
producen nuevos datos históricos y hacemos cambios al modelo, nuestras
estimaciones cambian, sería ridículo esperar lo contrario. Una vez más,
no estamos tratando de pronosticar si va a llover o no mañana, estamos
tratando de modelar un fenómeno socioambiental complejo y rápidamente
cambiante. No actualizar nuestro trabajo sería erróneo. En este caso,
dado que el modelo no considera retrasos de información dinámicos (i.e.,
conforme incrementa el número de pruebas, los retrasos de información
son menores) es posible que nuestra estimación de casos reales tenga un
sesgo positivo. ¿Se deben dar estas cifras al público y a los tomadores
de decisiones? Sí, creo que eso es lo correcto, el público debe estar lo
más informado posible, ya que todos necesitamos tomar decisiones
personales y profesionales para manejar la pandemia. ¿Es la diferencia
entre el número real estimado y el número confirmado de casos y decesos
el resultado de una conspiración? No, no lo creo. He interactuado en los
últimos meses con varios analistas y funcionarios públicos que están
trabajando para atender la pandemia, y esa interacción sólo me confirma
el heroísmo y el profesionalismo de muchos de ellos. Sin embargo, la
realidad es que sin pruebas a gran escala, la incertidumbre sobre el
número real de muertes y casos aumenta, y con esto la diferencia entre
los casos confirmados y los reales. Este punto no ha sido explicado con
suficiente claridad al público.

Un indicador que se utiliza comúnmente para monitorear lo que está
sucediendo con la pandemia es la tasa de reproducción-R0-. En resumen,
este indicador describe el número de contactos infecciosos por período
de tiempo que cada persona infecciosa genera (i.e., cid), controlando
por la probabilidad de que las personas infectadas se encuentren con una
persona susceptible (i.e., S/N). El primer componente de este índice
depende de los contactos promedio entre las personas (c), la
probabilidad de infección después de estar en contacto con una persona
infecciosa (i) y la duración media de la infección (d). El segundo
componente de este índice depende de la población total (N) y la
población susceptible (S). Si R0 es mayor que uno, la difusión del
virus se está acelerando, si se encuentra por debajo de uno, la
propagación del virus se encuentra en una trayectoria hacia la
estabilización. Es importante tener en cuenta que cuando R0 es
aproximadamente uno, la situación es extremadamente frágil, ya que
cambios en cualquier dirección pueden dar lugar a resultados
completamente diferentes (i.e., este es un umbral de criticalidad). Por
lo tanto, un primer objetivo de contención es empujar R0 hacia uno, una
vez que se alcanza este hito, el objetivo debe ser a) mantener R0 cerca
de uno o b) seguir empujando R0 por debajo de uno.

La siguiente figura utiliza los resultados para la Ciudad de México como
ejemplo de cómo podemos experimentar con este modelo para entender con
más detalle la situación de COVID19 en México. El área sombreada azul
(izquierda) describe las condiciones históricas de la línea base
simulada descrita por tres variables: R0 (fila superior), casos
confirmados (fila media) e índice de movilidad (fila inferior). Esta
parte del análisis es principalmente descriptivo. En este caso es
posible ver que la tasa de reproducción del virus disminuyó
sustancialmente durante marzo, se mantuvo estable durante abril y mayo,
y comenzó a crecer durante la primera semana de junio. Vemos también que
R0 está correlacionado positivamente con el índice de movilidad que
utilizamos para calibrar el modelo -la adición de datos de movilidad nos
ha ayudado a reducir significativamente la varianza del proceso de
calibración-. Por lo tanto, el seguimiento de la movilidad de la
población parece ser un buen proxy de la velocidad a la que se está
reproduciendo el virus.

El área blanca (derecha) muestra los resultados del experimento de
simulación que utilizamos para comprender con más detalle el estado del
virus en la región. En este experimento simulamos el modelo 200 veces
(empleando el muestreo Latinhypercube) para explorar cómo pueden cambiar
las cosas en los próximos días si los parámetros de la línea base están
sesgados negativa o positivamente. El propósito de este experimento es
estudiar las implicaciones de una infectividad más alta/menor del virus,
retrasos de información más altos/menores y tasas de movilidad de
población más altas/más bajas en las tres variables mostradas.

![](./media/image3.png)

Estos resultados muestran que la progresión de la pandemia sigue siendo
muy incierta. Sin embargo, es posible discernir algunos patrones
interesantes. En la fila superior vemos que en algunos casos la tasa de
reproducción del virus alcanza un valor inferior a uno, mientras que en
la mayoría de los casos, la tasa de reproducción se mantiene por encima
de este umbral. Una inspección más detallada, siguiente figura, muestra
que el escenario en el que la tasa de reproducción disminuye más
drásticamente esta asociado con una tasa de infectividad
sustancialmente menor del virus (54% inferior a la estimada en la
calibración de referencia) y un nivel sustancialmente menor de movilidad
de la población (66% inferior a las tasas de movilidad antes del
comienzo del brote). Sin embargo, estas condiciones están asociadas con
un mayor número de casos confirmados (i.e, 61,521).

![](./media/image4.png)

 

Como se muestra en la figura siguiente, dado que el número confirmado de
casos es una versión retrasada del número real de casos, esto crea una
discrepancia que es muy difícil de digerir para el público y para los
tomadores de decisiones. En este caso, los resultados están filtrados
para mostrar solo los resultados de la simulación más optimista en el
experimento. La fila superior ahora muestra el número real estimado de
casos. Podemos ver claramente que en este caso, mientras el número real
estimado de casos se estabiliza, el número confirmado de casos continua
creciendo.

![](./media/image5.png)

 

Esta discrepancia es un enorme desafío de comunicación, si únicamente
empleamos el número confirmado de casos para informar al público sobre
el progreso realizado con la pandemia, el público ciertamente se sentirá
decepcionado y frustrado, ya que los resultados de las acciones de
contención solo se serán evidentes semanas después de que las medidas de
contención entren en vigor. Esto me parece enfatiza la importancia de
realizar pruebas. Se ha argumentado que las pruebas masivas pueden
ayudarnos a gestionar de mejor manera la pandemia por varias razones;
sin embargo, en México y otros países, aún hay funcionarios públicos que
se mantienen escépticos con respecto de la utilidad de pruebas masivas.
Creo que esto es un error. Es posible que sea atractivo reducir el
número de pruebas para registrar un menor número de casos y con ello
dar la impresión de que la pandemia está bajo control. La desventaja de
hacer esto es que entre menor sea el número de pruebas, mayor el tiempo
que tomará registrar públicamente el efecto de las acciones de
contención. Lo anterior puede generar grandes frustraciones en la
población.

El escenario descrito también es interesante porque muestra que es
posible reducir la tasa de reproducción del virus y estabilizar el
número de infecciones si la infectividad del virus y la movilidad de la
población se mantienen bajo control. Mantener a la gente en casa más
tiempo va a ser muy difícil dado que muchas personas necesitan
urgentemente volver al trabajo, pero reducir la infectividad del virus
se puede lograr en cierto grado usando tapabocas de manera generalizada,
lavándonos las manos con más frecuencia, manteniendo una distancia
segura cuando salimos y considerando el nivel de riesgo de diferentes
actividades económicas (e.g., este artículo proporciona un análisis
interesante y útil sobre este punto:
[<span class="underline">https://tinyurl.com/y9nffef5</span>](https://tinyurl.com/y9nffef5)
). En la Ciudad de México, al 2 de julio, el número de casos confirmados
asciende aproximadamente a 48 mil personas, un número inferior al
mostrado en el mejor escenario de nuestro experimento. Esto, sin duda es
una señal de que la tasa de reproducción del virus se redujo durante
junio, lo cual es definitivamente una buena noticia (necesitamos
actualizar el análisis para saber con mayor detalle que tan frágil es
realmente la situación en la Ciudad de México).

La figura siguiente resume el resto de los resultados del experimento
para todos los estados de la república. Las columnas denotan meses en el
calendario y las filas indican regiones. El número en las celdas indica
el porcentaje de simulaciones que logran la estabilización del brote
(R0\<=1) para el mes indicado. Por ejemplo, para la Ciudad de México,
este análisis muestra que el 20% de las simulaciones alcanzan la
estabilización en junio, el 30% en julio y el 37% en agosto. De tal
manera que, a lo largo de las 200 simulaciones, para septiembre de 2020,
el 87% de ellas logran la estabilización.

![](./media/image6.png)

Al analizar otros estados podemos ver que otras regiones están en una
fase similar a la de la Ciudad de México, estas son: Jalisco, Veracruz,
Sinaloa, Yucatán y Guerrero. Por el contrario, los estados que pueden
requerir un mayor periodo de tiempo para estabilizar el crecimiento de
la pandemia incluyen Colima, Baja California Sur, Morelos y Zacatecas.

 

Dado que la mayoría de los estados están considerando levantar
restricciones en este momento, es esencial entender el nivel de riesgo
que cada una de estas regiones enfrenta durante este proceso. Para
examinar esto, estimamos el impacto que tasas de movilidad más altas o
más bajas pueden tener en la tasa de reproducción del virus a nivel
regional.

La figura siguiente muestra esta última parte del análisis. Las columnas
denotan cambios en los rangos en las tasas de movilidad con respecto al
último punto registro disponible (6 de junio). Columnas de la derecha,
denotan conjuntos de escenarios en los que las tasas de movilidad
aumentan con respecto al comienzo de junio. A la izquierda, hay
escenarios en los que las tasas de movilidad disminuyen. La leyenda del
color y el valor en las celdas denotan la tasa media de reproducción del
virus del 6 de junio al 7 de julio.

 ![](./media/image7.png)

Estos resultados nos dan una idea de la probabilidad de que un estado
experimente una aceleración en la tasa de reproducción del virus a
medida que se levantan las restricciones (es decir, se experimentan
tasas de movilidad más altas). En este caso, los estados que son capaces
de absorber tasas de movilidad más altas son aquellos con un menor
riesgo de reapertura. En este sentido, el único estado que parece estar
en esta situación es Quintana Roo, para el que podemos ver que la tasa
media de reproducción del estado se mantiene por debajo de 1.4 mientras
las tasas de movilidad no aumenten más allá del 50% en comparación con
la condición de referencia. Otros estados, como la Ciudad de México,
deben ser cuidadosos al relajar las restricciones ya que un aumento de
las tasas de movilidad superior al 50% -con respecto de las condiciones
base- puede dar lugar a un aumento sustancial de la tasa de reproducción
del virus. Por último, estados como Zacatecas, San Luis Potosí, Puebla,
Estado de México, Colima y Guanajuato parecen enfrentar el mayor riesgo
de reabrir sus economías dado que, modestos aumentos en las tasas de
movilidad, pueden resultar en aumentos sustanciales en la tasa de
reproducción del virus.

Los resultados discutidos en esta nota muestran que estamos en un
momento frágil. La mayoría de los estados enfrentan a un camino difícil
hacia adelante para contener el virus. Mantener las restricciones de
distanciamiento social será cada vez más difícil porque muchas personas
necesitan urgentemente volver al trabajo. ¿Qué pasará en los siguientes
meses? Es imposible predecirlo. Usar nuestra energía para buscar formas
de describir la tragedia de manera más atractiva es una pérdida de
tiempo. En este momento, el análisis debe enfocarse en entender quién
está progresando, cómo lo hizo y emplear esas lecciones para ayudar las
regiones que más lo necesiten.
