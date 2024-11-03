
# Sistema de Recomendación de Videojuegos para Steam

## Descripción del Problema

Steam, una plataforma multinacional de videojuegos, busca mejorar la experiencia de sus usuarios mediante un sistema de recomendación de videojuegos. Sin embargo, los datos disponibles son crudos y desorganizados, lo que complica la creación de un modelo efectivo de Machine Learning. El objetivo de este proyecto es implementar un MVP (Minimum Viable Product) que integre procesos de **Data Engineering**, **Feature Engineering** y **desarrollo de una API** utilizando **FastAPI**.

Al analizar el contexto y la solicitud del cliente, se procede a revisar los datasets entregados y se realizan los siguientes pasos.

1. **Transformaciones**: En el notebook EDA se realiza los analisis de datos y la informacion sobre la distribucion de los mismos. en el ETL se realizan las trasnformaciones de los datos para el analsis de sentimientos y el sistema de recomendacion se eliminan columnas innecesarias del dataset y optimiza el rendimiento del modelo y de la API. se exportan archivos parquet para disminuir el peso del dataset. 
  
2. **Analsis de sentimiento**: Crea la columna `sentiment_analysis` en el dataset `user_reviews` utilizando análisis de sentimiento. se realiza con VaderSentiment el cual me funciono y dio el resultado esperado.

3. **Desarrollo de API**: Implementa una API RESTful utilizando FastAPI con las siguientes funciones:
    Se realizan las 5 funciones en el archivo main.py incluido los dos tipos de recomendaciones item_item y user_item a traves de la similitud del coseno ver archivo "sistema de recomendacion"
    para mi fortuna todas las funciones a nivel local eran productivas.

    ![alt text](<Captura de Pantalla 2024-10-15 a la(s) 5.59.33 p.m.-1.png>)

4. **Deployment**: Despues de dias de intentar deployar la API, fue imposible multiples errores me lo impidieron, trate de solucionarlo todo pero no fue posible, cuando una funcion parecio deployarse me aparecio un mensaje de falta de memoria del github, el cual trate de solucionar comprando mas memoria y haciendo otro repositorio pero no funciono. Incluso este README no alcanzo a hacer adherirse al repositorio.
 ![alt text](<Captura de Pantalla 2024-10-15 a la(s) 5.59.33 p.m.-1.png>)

Fue una experiencia enriquesedora y frustrante por que no pude lograr mi objetivo deployar lo logrado.