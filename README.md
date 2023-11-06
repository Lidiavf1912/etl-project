# etl-project

![](https://github.com/Lidiavf1912/etl-project/blob/main/imagenes/cabecera_readme.avif)

## Indice:
1.[Contexto](#Contexto)\
2.[Proceso de extracción y transformación](#Proceso_de_extracción_y_transformación)\
3.[Proceso de carga de datos](#Proceso_de_carga_de_datos)\
4.[Conclusiones y sugerencias](#Conclusiones_y_sugerencias)\
5.[Links y referencias](#Links_y_referencias)


## 1. Contexto <a name="Contexto"/>

El proyecto que se va a realizar se basa principalmente en analizar los productos de televisión OLED en la tienda de LG Outlet que se pueden encontrar [aquí](https://www.tiendalgonline.com/oled-tv-lg-outlet/).

Una vez analizados los productos y sus precios procederemos a comparar sus precios en una de sus empresas retailer: Mi Electro. 

Puedes acceder a su pagina web [aquí](https://www.mielectro.es/)

Además, se ha extraído un CSV de un informe de Kaggle en el que se encuentran las principales empresas competidoras en el sector de la televisión de LG Electronics, donde también aparecen características de los productos de televisión, sus precios de venta, valoraciónes de los clientes, etc. 

Puedes ver el informe de Kaggle [aquí](https://www.kaggle.com/code/devsubhash/tv-brands-market-analysis-eda)

## 2. Proceso de extracción y transformación <a name="Proceso_de_extracción_y_transformación"/>

Para realizar este proceso se han empleado los datos mencionados anteriormente. En los siguientes puntos se va a explicar más en detalle lo realizado:

### 2. 1 LG Outlet

Para analizar la tienda de LG Outlet y sus productos de televisión OLED he extraídos los datos siguientes:

- id

- nombre del producto

- precio real en tienda

- precio en tienda outlet

- descuento aplicado

- id para las empresas retailers

Para acceder al documento pulse [aquí](https://github.com/Lidiavf1912/etl-project/blob/main/python/lg%20outlet.ipynb)

### 2.2 Mi Electro

De la página web de Mi Electro he extraído los siguiente datos de los productos de TV Oled de LG Outlet que están disponibles en esta empresa:

- nombre con la descripción del producto

- precio en tienda

- precio rebajado

- descuento aplicado

Para acceder al documento pulse [aquí](https://github.com/Lidiavf1912/etl-project/blob/main/python/Mielectro.ipynb)

### 2.3 CSV tv brand

Para poder analizar las empresas competidoras he agrupado la tabla por marcas obteniendo el precio promedio de las televisiones que aparecían en el dataset y el ratio según sus clientes. Además, he creado una columna con el número de productos de cada marca que proporcionaba el dataset.

Para acceder al documento pulse [aquí](https://github.com/Lidiavf1912/etl-project/blob/main/python/csv%20tv%20brands%20market.ipynb)

## 3. Proceso de carga de los datos <a name="Proceso_de_carga_de_datos"/>

Una vez extraída y transformada la información se ha procedido a realizar la carga de los datos y sus relaciones en MySQL, se puede consultar la carga realizada [aquí](https://github.com/Lidiavf1912/etl-project/blob/main/python/esquema%20mysql.ipynb)

## 4. Conclusiones y sugerencias <a name="Conclusiones_y_sugerencias)"/>

Este proyecto ha sido elaborado como primera toma de contacto. En un futuro se prevee mejorar el contenido automatizando estos procesos para poder realizarlo de una forma menos pesada. Por otra parte, también se prevee analizar más empresas retailers de estos productos e incluso analizar más productos de la tienda LG Outlet. O sea, se prentendrá una expansión del proyecto tanto horizontal como verticalmente.

## 5. Links y referencias📂 <a name="Links_y_referencias"/>

[Pandas](https://pandas.pydata.org/docs/)

[Numpy](https://numpy.org/doc/1.18/)

[Python](https://docs.python.org/3/library/functions.html)

[Matplotlib](https://matplotlib.org/)



