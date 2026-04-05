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
