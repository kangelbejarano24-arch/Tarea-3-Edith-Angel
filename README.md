# Procesamiento en batch

## Descripción

Este proyecto realiza un análisis de datos en batch utilizando Apache Spark sobre un conjunto de datos de vehículos involucrados en accidentes de tránsito en el municipio de Tuluá.

El dataset incluye:
- Marca del vehículo
- Modelo del vehículo
- Tipo de vehículo
- Edad del vehículo
- Fecha del accidente
- Gravedad del accidente
- Departamento del accidente
- Municipio del accidente
- Autoridad de tránsito

El objetivo es identificar patrones en los accidentes.

## Tecnologías utilizadas

- Apache Spark
- Python (PySpark)
- Hadoop HDFS

## Procesamiento realizado

### 1. Carga de datos
Se carga el dataset desde HDFS.

### 2. Limpieza de datos
- Eliminación de valores nulos
- Eliminación de duplicados

### 3. Transformación
- Creación de la columna "año_accidente"

### 4. Análisis exploratorio (EDA)
- Vehículos con más de 10 años
- Cantidad de accidentes por tipo
- Cantidad por gravedad
- Marcas más involucradas

## Ejecución

1. Cargar dataset en HDFS:
hdfs dfs -put /home/hadoop/anem-hgsc.csv /Tarea3EdithAngel 

2. Ejecutar:
python3 tarea3_edith_angel.py

## Resultados

- Las motocicletas presentan más accidentes
- La mayoría son con heridos
- Marcas como Yamaha y Honda son frecuentes

## Autor

Edith Karina Angel Bejarano

# Procesamiento en Batch

## Descripción del proceso

El procesamiento en batch se realizó utilizando Apache Spark, cargando un dataset de accidentes de tránsito desde HDFS.

## Etapas del procesamiento

### Carga de datos

Se cargó el archivo CSV desde HDFS usando Spark DataFrames.

### Limpieza de datos

Se eliminaron valores nulos y registros duplicados para garantizar la calidad de los datos.

### Transformación

Se creó una nueva columna llamada `anio_accidente` para facilitar el análisis temporal.

### Análisis exploratorio (EDA)

Se realizaron consultas como:

* Filtrado de vehículos antiguos
* Conteo por tipo de vehículo
* Análisis de gravedad
* Ranking de marcas

## Resultados

Se identificó que:

* Las motocicletas son el tipo de vehículo con más accidentes
* La mayoría de los accidentes son con heridos
* Algunas marcas aparecen con mayor frecuencia

## Conclusión

El uso de Spark permitió procesar eficientemente el dataset y obtener información relevante para el análisis de accidentes de tránsito.

# Procesamiento en Batch con Apache Spark

## Descripción

Este proyecto realiza un análisis de datos en batch utilizando Apache Spark sobre un conjunto de datos de vehículos involucrados en accidentes de tránsito en el municipio de Tuluá.

El objetivo es identificar patrones en la siniestralidad vial, como los tipos de vehículos más involucrados, la gravedad de los accidentes y las marcas con mayor frecuencia.

## Dataset

Fuente: Datos Abiertos de Colombia
Archivo: anem-hgsc.csv

Variables principales:

* Marca del vehículo
* Modelo
* Tipo de vehículo
* Edad del vehículo
* Fecha del accidente
* Gravedad del accidente
* Ubicación

## Tecnologías utilizadas

* Apache Spark
* Python (PySpark)
* Hadoop HDFS

## Procesamiento realizado

### 1. Carga de datos

Se cargan los datos desde HDFS utilizando Spark DataFrames.

### 2. Limpieza de datos

* Eliminación de valores nulos
* Eliminación de registros duplicados

### 3. Transformación de datos

* Creación de la columna `anio_accidente` a partir de la fecha

### 4. Análisis exploratorio (EDA)

* Vehículos con más de 10 años
* Ordenamiento por antigüedad
* Conteo por tipo de vehículo
* Conteo por gravedad
* Ranking de marcas

## Ejecución

1. Subir dataset a HDFS:

```
hdfs dfs -put /home/hadoop/anem-hgsc.csv /Tarea3EdithAngel
```

2. Ejecutar el programa:

```
python3 tarea3_edith_angel.py
```

## Resultados principales

* Las motocicletas presentan mayor número de accidentes
* La mayoría de los accidentes son con heridos
* Marcas como Yamaha, Honda y Chevrolet son las más frecuentes

## Autor

Edith Karina Angel Bejarano
