Algunos factores asociados con fallecimientos y hospitalizaciones por covid19

Alejandro Díaz Domínguez \*

A continuación, se presenta una sencilla aplicación de aprendizaje
máquina para clasificar factores que inciden en fallecimientos y
hospitalizaciones por covid19 en México. Para conocer dichos factores se
empleó un algoritmo de aprendizaje máquina no supervisado, cuyos
comandos se contienen en la librería *rpart* en el paquete estadístico R
(Therneau, Atkinson y Ripley 2019).

Primero se estimó un árbol de decisión con el método de clasificación,
puesto que se trató de una variable dependiente binaria. El aprendizaje
máquina no supervisado (*unsupervised machine learning*) emplea un
algoritmo previamente entrenado, el cual ya ha sido automatizado, por lo
cual ya no requiere de monitoreo (Díaz Domínguez 2020: 1-2, 8).

Aunque los árboles de decisión suelen ser mucho más sensibles a la
información recibida que otras técnicas (como por ejemplo el bosque
aleatorio o *random forest*), los resultados iniciales sugieren
elementos que resultan lógicos y hasta cierto punto esperados. Para
conocer mejor el comportamiento de las variables más relevantes, también
se estimaron modelos *random forest* con 500 árboles aleatorios usando
la librería *random forest* (Liaw y Wiener 2018).

**Fallecimientos**

La base incluyó todas las personas que recibieron resultado positivo en
la prueba sobre el covid19, esto es 35,022 del gran total de 130,956 que
fue reportado el 10 de mayo pasado por la Secretaría de Salud, esto es
el 27 por ciento.

Se procedió a estimar el modelo de clasificación en el 70 por ciento de
la muestra, esto es, 24,516 casos, dejando el 30 por ciento restante
para verificar que tan acertada fue la clasificación. El modelo parece
contar tiene con una capacidad de predicción adecuada, siendo del 90.6
por ciento (ente 90 y 91.2 por ciento). Dicha exactitud (*accuracy*) se
obtiene de dividir las observaciones correctamente pronosticadas entre
el total. En otras palabras, el modelo clasifica incorrectamente el 12
por ciento de los casos.

En la gráfica 1, la cual muestra las ramas más relevantes del árbol (con
un parámetro de complejidad -*complex parameter*-no menor a 0.018 para
no sobreajustar los datos, evitando con ello el forzar indebidamente la
inclusión de ramas adicionales, las cuales ya no aportarían a una mejor
clasificación), se observan los factores con mayor incidencia en
fallecimientos por covid19 en México. De entre las personas que dieron
positivo a la prueba covid19, el primer factor que destaca es si la
persona fue o no fue hospitalizada. Si no fue hospitalizada, esto es, si
se trató de pacientes de carácter ambulatorio, la probabilidad de
fallecimiento es del 2 por ciento.

Figura 1. Árbol de clasificación, fallecimientos por covid19 en México

![](./media/image1.jpeg)

Si la persona fue hospitalizada pero no fue intubada, la probabilidad es
del 19 por ciento. Ahora bien, si la persona fue hospitalizada y además
fue intubada, la probabilidad variará dependiendo del lugar de la unidad
médica donde fue atendida. Si era atendida en Ciudad de México, fuera de
una unidad de cuidados intensivos, entonces la probabilidad de fallecer
era del 28 por ciento. Si estaba hospitalizada, fue intubada, se hallaba
en Ciudad de México y se encontraba en una unidad de cuidados
intensivos, entonces la probabilidad de fallecimiento era del 59 por
ciento. Finalmente, si la persona estaba hospitalizada, se encontraba
intubada y era atendida por una unidad médica fuera de la Ciudad de
México, entonces la probabilidad de fallecimiento era del 61 por
ciento.

La sensibilidad del modelo (*sensitivity*) es del 98.3 por ciento, el
cual se calcula al dividir los casos pronosticados como personas vivas
entre todas las personas vivas. Sin embargo, la especificidad es baja
(*specificity*), del 20.3 por ciento, la cual se obtiene al dividir los
casos pronosticados como personas fallecidas entre todas las personas
fallecidas. En contraposición, el valor de los casos pronosticados como
vivos es igual a 91.8 por ciento y el de los fallecidos es 56.9 (*pos
pred value* y *neg pred value*).

En síntesis, si bien el modelo presenta un *F1 score* del 94.9, el cual
conjunta la relación entre precisión y sensibilidad, sin duda requiere
mejorarse. Con todo, la estimación parece arrojar algunas perspectivas
medianamente útiles sobre los factores asociados con fallecimientos por
covid19. Entre ellos, la innegable relevancia de estar o no en
hospitalización, la de estar o no con un respirador y de permanecer en
una unidad de cuidados intensivos. En menor medida, también importa el
lugar donde se atiende a pacientes de covid19, esto es, si se trata o no
de la Ciudad de México.

Adicionalmente, se corrió un modelo *random forest* con 500 árboles
aleatorios con la misma base reportada el 10 de mayo, empleando también
todos los casos positivos por covid19, donde se encontraron como
variables más importantes intubación, hospitalización, edad, neumonía y
el estar en una unidad de cuidados intensivos.

**Hospitalización**

Desde luego que estos hallazgos se conectan con otros modelos de
clasificación, como el de personas hospitalizadas. Para este modelo se
emplearon los datos abiertos reportados el 24 de abril. El hallazgo
esperado se centró en si la persona reportaba neumonía. Se estimó un
árbol de decisión para clasificar la variable binaria hospitalización,
también separando la muestra en un 70 por ciento para entrenamiento y en
un 30 por ciento como prueba para conocer qué tan bien pronostica el
modelo.

Los resultados se aprecian en la figura 2. Al presentar neumonía, la
probabilidad de hospitalización fue del 87 por ciento. Por otro lado, si
la persona no reportaba neumonía, era de 65 o más años y fue
inicialmente atendida por un hospital distinto a los del sector salud,
la probabilidad de ser internada fue 60 por ciento. Ahora bien, si no
reportaba neumonía, tenía 65 o más años y fue inicialmente atendida en
un hospital del sector salud, entonces la probabilidad de ser internada
fue 16 por ciento. Finalmente, si la persona no reportaba neumonía y era
menor a 65 años, entonces la probabilidad de ser internada era del 10
por ciento.

En dicho árbol de clasificación, la exactitud era del 88.2 por ciento
(entre 87.8 y 88.7), la sensibilidad del 95.3 por ciento y la
especificidad del 67.4 por ciento. Al correr un modelo *random forest*
con 500 árboles aleatorios, se encontró una importancia similar entre
variables, tales como neumonía, edad, unidad médica del Sector Salud,
diabetes, hipertensión, epoc, unidad médica del IMSS, del ISSSTE y
hospitales privados. Adicionalmente, el modelo *random forest* para
clasificar hospitalización presentó una sensibilidad del 89.6, una
especificidad del 83.9 (es decir, se apreció una notoria mejoría) y una
exactitud del 88.4 (entre 87.9 y 88.9 por ciento).

Figura 2. Árbol de clasificación, hospitalizaciones por covid19 en
México

![](./media/image2.tiff)

**Conclusiones preliminares**

Los modelos de clasificación revelaron la importancia de variables como
neumonía, hospitalización, edad, respiradores y unidades de cuidados
intensivos. Aunque se requiere trabajo teórico y empírico adicional para
conocer mejor los factores asociados con fallecimientos y
hospitalizaciones por covid19 en México, los modelos presentados
parecieran reflejar diversas intuiciones y discusiones sobre la
importancia de neumonía y respiradores.

Si bien estos modelos son susceptibles de mejora, lo que quizá sí
sugieren es la urgente necesidad de analizar y estudiar de manera
razonablemente sistemática la información disponible, de modo tal que se
pueda actuar de manera pronta ante los retos que ya se tienen ante lo
inédito de esta pandemia.

\* Alejandro Díaz Domínguez es doctor en Ciencia Política por la
Universidad de Vanderbilt y profesor de la Escuela de Gobierno del
Tecnológico de Monterrey (@alejdiazd)

(1) Therneau, Terry, Beth Atkinson y Brian Ripley. 2019. *Package
‘rpart’ (Recursive Partitioning and Regression Trees)*. R CRAN
\[https://CRAN.R-project.org/package=rpart\]

(2) Díaz Domínguez, Alejandro. 2020. “How Futures Studies and Foresight
Could Address Ethical Dilemmas of Machine Learning and Artificial
Intelligence”. *World Futures Review* 12(2): 169-180.
<https://doi.org/10.1177/1946756719894602>

(3) Liaw, Andy and Matthew Wiener. 2018. *Package ‘randomForest’
(Breiman and Cutler's Random Forests for Classification and
Regression)*. R CRAN
\[https://cran.r-project.org/web/packages/randomForest/randomForest.pdf\]
