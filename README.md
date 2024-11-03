
# Sistema de Recomendación de Videojuegos para Steam

## Descripción del Problema

Steam, una plataforma multinacional de videojuegos, busca mejorar la experiencia de sus usuarios mediante un sistema de recomendación de videojuegos. Sin embargo, los datos disponibles son crudos y desorganizados, lo que complica la creación de un modelo efectivo de Machine Learning. El objetivo de este proyecto es implementar un MVP (Minimum Viable Product) que integre procesos de **Data Engineering**, **Feature Engineering** y **desarrollo de una API** utilizando **FastAPI**.

Al analizar el contexto y la solicitud del cliente, se procede a revisar los datasets entregados y se realizan los siguientes pasos.

1. **Transformaciones:** En el notebook de Exploración de Datos (EDA), se realizan análisis de los datos de las 3 bases de datos y se proporciona información sobre su distribución. En la etapa de ETL, se llevan a cabo las transformaciones necesarias en los datos para el análisis de sentimientos y el sistema de recomendación. Esto optimiza tanto el rendimiento del modelo como el de la API. Además, se exportan archivos en formato Parquet para reducir el tamaño del dataset.
![Código](imagen/Captura_transf)

2. **Machine Learning:** Se lleva a cabo un análisis de sentimiento en el archivo user_reviews utilizando la biblioteca VaderSentiment. Como resultado de este análisis, se genera la columna sentiment_analysis en el dataset user_reviews.
![Código](imagen/Captura_Codigo_ana.png)
![Resultado](imagen/Captura_Analisis.png)


1. **Desarrollo de API:** Se implementa una API RESTfull utilizando FastAPI, que incluye 7 funciones en el archivo main.py. Las dos últimas funciones abarcan dos tipos de recomendaciones: item-item y user-item, basadas en la similitud del coseno, como se detalla en el archivo "sistema de recomendación". 
Se crea un entorno virtual para probar la API localmente 
![Imagen](imagen/Captura_fastapi.png)
![Imagen](imagen/Captura_api_local.png)


2. **Deployment**: 


