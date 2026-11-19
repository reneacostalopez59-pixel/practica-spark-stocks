# Práctica Apache Spark Standalone — Análisis de `stocks.txt`

- **Alumno:** René Nicolas Acosta López
- **Matrícula:** 125052937
- **Entorno:** BDA Lab (Docker con Hadoop, HDFS, Apache Spark y Jupyter Notebook)

## Descripción del proyecto

Implementación de un flujo completo de procesamiento distribuido con **PySpark y RDDs** (SparkSession, SparkContext, `map`, `filter`, `reduceByKey`, `aggregateByKey`, `sortBy` y `saveAsTextFile`) siguiendo los 6 pasos de la práctica de Spark Standalone.

> **Nota sobre el dataset:** El archivo oficial `stocks.txt` descargado de `josepgarcia/datos` contiene 30 registros de inventario de productos con el esquema `id,name,category,quantity,price` (31 líneas incluyendo encabezado). El análisis se adaptó a este esquema real conservando todas las transformaciones, agregaciones, cálculos de dispersión/volatilidad y acciones requeridas.

## Evidencia de ejecución
Particiones del RDD: 2 particiones (rdd_raw.getNumPartitions()).

Resultados completos y Preguntas de Reflexión: Disponibles directamente al abrir practica_spark_stocks.ipynb.

## Estructura del repositorio

```text
practica-spark-stocks/
├── practica_spark_stocks.ipynb   # Notebook completo con código, salidas y reflexión
├── DATOS/
│   └── stocks.txt                # Dataset utilizado
├── RESULTADOS/
│   ├── volumen_por_producto/     # Salida de saveAsTextFile()
│   └── stats_por_categoria/      # Salida de saveAsTextFile()
└── img/
    └── spark_ui.png              # Evidencia de ejecución en Spark UI (puerto 4040)
