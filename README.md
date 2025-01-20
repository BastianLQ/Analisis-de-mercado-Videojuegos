# Análisis y pronóstico de mercado: Ice Games
__Análisis del mercado de los videojuegos, visualización de datos avanzada, análisis exploratorio y estadístico, prueba de hipótesis__

<image src="https://github.com/BastianLQ/Analisis-de-mercado-Videojuegos/blob/main/Images/banner.png" alt="Collage de gráficos">

_Para ver proyecto desarrollo en código hacer click [aquí](https://portfoliodabastianlopez.on.drv.tw/Portafolio/P6.html)_

## Descripción del proyecto
Este proyecto se enfoca en analizar datos del mercado de los videojuegos (hasta 2016) para entender las tendencias en la preferencia de juegos por consola, realizar predicciones sobre consolas dominantes, y llevar a cabo un análisis estadístico de las ventas de juegos. Además, se calculó la correlación entre calificaciones y ventas, se analizaron diferencias entre juegos de géneros populares e impopulares, y se trazó un perfil de consumidor para tres regiones importantes. Finalmente, se realizaron dos pruebas de hipótesis para validar los hallazgos. Todo lo anterior se realiza con el fin de detectar oportunidades y juegos prometedores para el año 2017.
  
## Herramientas Utilizadas
- __Lenguaje de Programación:__ Python.
- __Entorno de Desarrollo:__ Jupyter Notebook.
- __Bibliotecas:__ Pandas, Numpy, Matplotlib, Seaborn, Scipy, Math.
  
## Proceso del Proyecto
- __Preanalisis de los datos:__ Esta fase contempló todos los preparativos, importación de librerías, limpieza, etc. que se realizaron antes de empezar con el análisis.
- __Análisis de los datos:__ En esta fase se desarrolló el grueso del proyecto, es decir, se respondieron las principales preguntas formuladas al inicio.
  - __Análisis exploratorio de datos:__ Aquí se exploró información sobre los juegos lanzados por año, el comportamiento general de los lanzamientos y las plataformas que podrían ser rentables para el 2017.
  - __Correlación:__ Se analizó la correlación entre calificaciónes (de usuarios y de la crítica) y ventas de juegos de PS4.
  - __Plataformas populares:__ Se eligieron juegos populares y se comparó la venta entre distintas plataformas.
  - __Géneros populares:__ Se hicieron divisiones según la popularidad de los géneros y se compararon las calificaciones (de la crítica y de usuario) entre los grupos.
- __Perfil de usuario para cada región:__ Se analizaron los de consumo de videojuegos de cada región estudiada (norteamérica, unión europea y japón).
- __Pruebas de hipótesis:__ Usando pruebas de Mann-Whitney, se comprueban estadísticamente dos hipótesis planteadas al inicio del informe sobre el consumo de videojuegos.
- __Resultados:__ Al final del informe se rescatan las conclusiones más importantes encontradas durante el desarrollo del proyecto.
  
## Descubrimientos revelantes
### Juegos lanzados por año

<image src="https://github.com/BastianLQ/Analisis-de-mercado-Videojuegos/blob/main/Images/output_38_0.png" alt="gráfico">

Se observa la cantidad de videojuegos lanzados por año, podemos apreciar que desde 1995 se superan los 200 juegos lanzados por año y que desde el 2001 se superan los 400, haciendo que los datos recopilados sean significativos para un análisis. Además podemos notar un periodo record en 2008 y 2009, en donde se lanzaron más de 1400 juegos a la venta.

### Análisis de plataformas

<image src="https://github.com/BastianLQ/Analisis-de-mercado-Videojuegos/blob/main/Images/output_42_0.png" alt="gráfico">

A partir del gráfico anterior se seleccionaron las 5 primeras plataformas (por ser las más rentables en cuanto a venta de videojuegos) y se analizaron, por año, el ingreso de cada una.

<image src="https://github.com/BastianLQ/Analisis-de-mercado-Videojuegos/blob/main/Images/output_44_0.png" alt="gráfico">

Del presente gráfico se puede apreciar que las plataformas de PlayStation, Xbox y la Nintendo DS, __se demoran entre dos a tres años en tomar una posición sólida en el mercado, donde se mantienen por entre cuatro a cinco años__. La Nintendo Wii se muestra como una excepción, ya que muestra un peak muy alto en 2009 y después se desploma brúscamente.

Tomando en cuenta la información recolectada anteriormente, __se analizarán los juegos lanzados desde 2013 en adelante, de esta forma podremos saber qué plataformas están en camino a despegar, cuales no lo están haciendo, y cuales están bajando su popularidad__.

### Plataformas potencialmente rentables
Se visualizarán las ventas históricas de juegos de las 5 consolas más populares entre 2010 y 2015, las que vayan en tendencia ascendente serán consideradas como potencialmente rentables.

<image src="https://github.com/BastianLQ/Analisis-de-mercado-Videojuegos/blob/main/Images/output_52_0.png" alt="gráfico">

El gráfico muestra que __las plataformas potencialmente rentables son PS4 y Xbox One__, que han ido subiendo en ventas desde 2013 y se espera que lo sigan haciendo hasta tomar una posición sólida en el mercado, la nintendo 3DS ha ido bajando paulatinamente sus ventas, sin embargo, en 2015 sigue siendo la tercera plataforma mas exitosa en ventas de juegos. 

__En el caso de PS3 y Xbox 360, podemos ver una caída rápida desde que aparecen las sucesoras (PS4 y Xbox One), lo que puede significar que serán plataformas muy exitosas hasta que sean reemplazadas por sus respectivas sucesoras__ en 2019/2020 aproximadamente, tomando en cuenta que entre el lanzamiento de PS2 y PS3 hay 6 años, y entre PS3 y PS4 hay 7 años de diferencia. En el caso de Xbox, entre la 360 y la One también hay 7 años de diferencia.

### Ventas de todos los juegos
Podemos explorar estadísticamente en los siguientes gráficos de caja.

<image src="https://github.com/BastianLQ/Analisis-de-mercado-Videojuegos/blob/main/Images/output_58_0.png" alt="gráfico">

<image src="https://github.com/BastianLQ/Analisis-de-mercado-Videojuegos/blob/main/Images/output_58_1.png" alt="gráfico">

- El promedio de ventas de un juego vendido por esta tienda es de $488.000 dólares, y la mediana de $110.000 dólares.

En cuanto a las ventas totales, __se observa una media muy superior a la mediana y una distribución que nos indica que la proporción de valores atípicos es muy baja, sin embargo estos soy muy altos__. Los calulos indical que de todos los juegos lanzados a la venta entre 2013 y 2016 __un 12% superó el millon de dólares en ventas y apenas un 1% superó los 5 millones__.

Para continuar con el análisis de la distribución de ventas, se presentan gráficos de dispersión y de caja por plataforma para las consolas más populares.

<image src="https://github.com/BastianLQ/Analisis-de-mercado-Videojuegos/blob/main/Images/output_60_0.png" alt="gráfico">

<image src="https://github.com/BastianLQ/Analisis-de-mercado-Videojuegos/blob/main/Images/output_62_0.png" alt="gráfico">


## Ejecuta el proyecto [aquí](https://portfoliodabastianlopez.on.drv.tw/Portafolio/P6.html)
Para ver el diccionario de datos, el desarrollo completo en código, todos los gráficos y las conclusiones, haga click en el enlace de arriba
