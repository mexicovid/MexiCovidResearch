Curvas epidémicas por estado para casos positivos: promedios móviles a 7
días

Alejandro Díaz Domínguez \*

La medición del número de casos positivos día a día no permite observar
rezagos en captura, mientras que un horizonte semanal, es decir, de
siete días, incrementa las posibilidades de considerarlo.
Adicionalmente, dividir la información por entidad federativa permite
apreciar si existen curvas epidémicas distintas, debido a que algunos
estados pueden enfrentar mayores complicaciones, mientras que algunos
otros ya tuvieron que enfrentar tales problemas.

Para conocer curvas epidémicas que capturen estas variaciones, se
calcularon promedios móviles de siete días para cada de las entidades
federativas y a nivel nacional. Un promedio móvil es método de
descomposición en series de tiempo, que se emplea para estimar el ciclo
- tendencia de un conjunto de datos, los cuales deben ser compilados de
la misma forma y con la misma frecuencia, en este caso, diaria.

Para obtener un promedio móvil se calcula el promedio de los datos de la
serie en un número determinado de periodos. Con ello, se busca reducir
la parte de aleatoriedad de los datos, para dejar un componente de
ciclo-tendencia mucho más suave (Hyndman y Athanasopoulos 2018: sección
6.2).

Para ello se empleó el paquete estadístico R, de acceso gratuito y las
librerías *tseries* y *forecast* para declarar 33 series diarias del
primero de enero al 15 de mayo de 2020, considerando siete días sobre el
número de casos positivos reportados de forma diaria por la Secretaría
de Salud. Estos promedios móviles se calcularon sin centrarse.

Para cada una de las 33 curvas se incluyeron los datos de casos
positivos diarios en gris y el promedio móvil de siete días en rojo. Se
muestran dos paneles, uno que va de Aguascalientes a Michoacán (Gráfica
1) y otro que va de Morelos a Zacatecas, más la curva nacional (Gráfica
2).

Gráfica 1. Promedios móviles a 7 días, Aguascalientes a Michoacán

![](./media/image1.png)

Fuente: reportes diarios de la Secretaría de Salud.

La curva en color rojo muestra la tendencia suavizada de los datos
reportados diarios sobre casos positivos por Covid 19. Lo que se busca
es explorar el comportamiento de dicho promedio móvil, de modo que se
aprecie si la curva aún se muestra en su fase de crecimiento rápido o si
ya ha alcanzado su fase logarítmica.

Gráfica 2. Promedios móviles a 7 días, Morelos a Zacatecas y nacional

![](./media/image2.png)

Fuente: reportes diarios de la Secretaría de Salud.

La curva nacional no parece haber dejado la fase de crecimiento rápido,
como también se observa en la Ciudad de México, Guerrero y Sonora, entre
otras entidades, mientras que en algunos estados parece que quizá ya se
ha alcanzado la fase logarítmica. Sin embargo, en días recientes se han
manifestado nuevos incrementos, los cuales ya han sido capturados por el
propio promedio móvil con corte al 15 de mayo. Parece ser el caso de
Baja California Sur, Chihuahua, Nayarit, Quintana Roo y Zacatecas, entre
otras entidades donde la disminución se empieza a notar, aunque también
se observan datos al alza después del ya referido descenso.

En síntesis, la variación subnacional importa, pues en efecto, como en
otros aspectos, también en la fase de contagios existen “muchos
Méxicos”. Esta variación no sólo se intenta capturar con la división
por entidades federativas, sino también mostrando la propia escala de
cada entidad federativa, a efecto de apreciar tanto las trayectorias de
cada promedio móvil como su impacto en el número de casos positivos.

Desde luego que estos análisis podrían replicarse a nivel local, al
menos a nivel municipal. Una reflexión sobre los datos sería que están
sujetos a revisiones por parte de la propia autoridad y que dependen en
alguna medida del número de pruebas reportadas en los datos oficiales.
Con todo, es la información oficial disponible de manera pública, la
cual puede y debe ser analizada para ofrecer un panorama un poco más
completo, hasta donde sea posible, de lo que acaece con la pandemia en
México.

\* Profesor de la Escuela de Gobierno del Tecnológico de Monterrey.

Hyndman, R.J., y Athanasopoulos, G. 2018. *Forecasting: principles and
practice*. 2a ed, OTexts: Melbourne, Australia. \[OTexts.com/fpp2\].
Acceso en \<21 de mayo de 2020\>.
