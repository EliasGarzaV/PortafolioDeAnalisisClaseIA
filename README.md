# PortafolioDeAnalisisClaseIA

Este es el repositorio de Análisis en donde encontraran las actividades relacionadas con la clase de Inteligencia Artificial. Cabe recalcar que se trabajaron varias bases de datos por lo que esta la información tanto de la parte de Machine Learning como la de estadistica en este repositorio. 

## Entregables

- [Entregable Analisis de NOrmatividad: 11/09/2023](Entregables/AnalisisNormatividad.ipynb) - Aqui se encuentra el reporte sobre el contexto y normatividad de datos. 

- [Entregable Final Machine Learning: 11/09/2023](Entregables/EntregableFinal.ipynb) - Este es el resultado final con la concatenación de las entregas con todas las correcciones hechas para el módulo de Machine learning. Contiene la aparte de implementación asi como la última entrega de Análisis para las cuales se utilizó el mismo modelo. (*Si usted es el profesor Ivan este es el archivo bueno por ver*)


```
📦PortafolioDeAnalisisClaseIA
 ┣ 📂Data
 ┃ ┣ 📜precios_autos.csv
 ┃ ┗ 📜precios_autos_Diccionario.xlsx
 ┣ 📂Entregables
 ┃ ┣ 📜EntregableFinal.ipynb
 ┃ ┣ 📜Fase1.html
 ┃ ┣ 📜Fase1.ipynb
 ┃ ┣ 📜Fase1.pdf
 ┃ ┣ 📜Fase2.html
 ┃ ┣ 📜Fase2.ipynb
 ┃ ┣ 📜Fase2.pdf
 ┃ ┗ 📜Fase3.ipynb
 ┗ 📜README.md
```

## Sobre el problema y los datos de Machine Learning

Tenemos un  problema de regresión con datos de profesores en una universidad con los cuales vamos a intentar predecir su salario. Tenemos un rango de variables como lo son su puesto actual, la materia que imparten, la cantidad de años desde que obtuvieron su doctorado, los años que llevan trabajando y su sexo. Asimismo, tambien tenemos la columna del salario de profesores para hacer la prueba. Este dataset lo pueden encontrar en [Datos_Salariales](Data/salary.csv).

## Modelado

En cuanto al modelo utilizado tenemos varias pruebas. Inicialmente haremos una regresión lineal tanto de la forma optima con mínimos cuadrados (el dataset no es muy grande asi que en este caso es la mejor opción ya que tenemos suficiente memoria para los cálculos) como a traves de un optimizador el cual intentará ir moviendo los valores de los coeficientes para llegar a un óptimo local.  

Posteriormente veremos que tal funciona otro modelo como arboles de regresión o xgboost. 

## Sobre los cambios y correcciones

### Implementación
Los siguientes son las correcciones que se le han aplicado a este documento a partir de la retroalimentación del profesor para el caso del portafolio de Implementación:

 - Añadir contexto sobre la base de datos y link en el `README.md` de este repositorio.
 - Añadir descripción del modelo utilizado en el `README:md`
 - El reporte ahora incluye la descripción de los datos asi como el nombre. 
 - Tenemos ahora el reporte generado de exploración de datos. 
 - Al inicio del reporte tenemos la explicación de que es un problema de regresión. 
 - Ahora se añade los resultados del conjunto de entrenamiento además del de pruebas.
 - El modelo ahora contiene pruebas ademas de las de entrenamiento (el testing al final)
 - Ahora se hace la comparación con residuales y la diferencia entre los resultados. 
 - Ahora se varian diversos hiperparámetros al momento de generar las pruebas. 

### Análisis
Asimismo, para la entrega de Análisis tenmos los siguientes cambios (excluyendo cambios redundantes que ya se hicieron para la parte de implementacion):

 - Ahora separamos los datos en entrenamiento-validación-pruebas en una proporción 64:16:20. 
 - Hacemos todas nuestras pruebas con el conjunto de validación. El de pruebas es solo al final para revisar la evaluación final del modelo. 
 - Hacemos una busqueda para optimizar los hiperparámetros del modelo de gradiente descendiente estocastico. Variamos el learning rate inicial, el parametro de regularización, la función de error y las iteraciones máximas. 
 - Analizamos el sesgo comparando las métricas de nuestros 3 conjuntos de datos y tenemos la tabla de diferencias entre nuestros conjuntos de entrenamiento y validación para el caso del gradiente descendiente. 
 - La varianza ahora la podemos ver a través de los diagramas de residuos de nuestros modelos los cuales se encuentran en la evaluación. 
 - Comparamos las metricas de los conjuntos para concluir que no tenemos un overfitting alto. 
 - En nuestro modelo de gradiente descendiente añadimos una regularización del tipo 'l1' para mejorar los resultados. 
 

