# Series Temporales en R

![banner_serie_temporal](img/banner.png)

## Introducción

Esta tarea personal sirve para la puesta en práctica del estudio de series temporales. 
He descargado un conjunto de datos de la página web de [Kaggle](https://www.kaggle.com/datasets/sudalairajkumar/daily-temperature-of-major-cities) que contiene los valores de temperatura media diaria de las principales ciudades del mundo. Dichas temperaturas son recogidas en Fahrenheit desde el 1 de enero de 1995 hasta el 13 de mayo de 2020. 

Las características más importantes a tener en cuenta para nuestro estudio son las siguientes:

- **Region**: Nombre de la región.
- **Country**: País.
- **State**: Nombre del estado (en caso de tenerlo).
- **City**: Nombre de la ciudad
- **Month**: Número del mes. 
- **Day**: Número del día.
- **Year**: Año al que pertenece la medida.
- **AvgTemperature**: Temperatura promedio de la entrada.

El objetivo de este estudio es intentar predecir la tendencia de temperatura en los próximos años. Como el tamaño de los datos es excesivamente grande, voy a filtrar y focalizar el estudio en una ciudad en concreto. 

Para esta tarea, recogeremos el primer valor de temperatura de cada mes de la ciudad de Madrid desde el año 2000 hasta el 2014 incluido. En estos 14 años de datos encontramos un total de 168 observaciones para estudiar. Para la predicción hay margen hasta el 2020, pero con intentar predecir las siguientes 12 observaciones tenemos suficientes (lo que equivale predecir al año 2015 en su totalidad).

## Representación gráfica, descomposición y análisis de los datos

Al seleccionar el primer valor de cada mes, se nos queda una un conjunto de periodo
12. Si visualizamos nuestros datos observamos que tienen una media constante y una varianza
acotada. 

![meteorite logo](img/1_Valores_temperatura.png)

