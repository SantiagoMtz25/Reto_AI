La presentación esta en el archivo de Titanic Classification.
El ejecutable es Titanic_Reto.

Link a Collab:

https://colab.research.google.com/drive/1CzPraXJDs5TGaXDrWv_aE4OtFGPOSNl3?usp=sharing

Link a Youtube:

https://youtu.be/aYYxbzGhE_Q?feature=shared


Predicción de Supervivencia en el Titanic
1. Visión General del Proyecto
Este proyecto forma parte de un desafío de aprendizaje automático centrado en predecir qué pasajeros sobrevivieron al desastre del Titanic utilizando el conjunto de datos del Titanic. El conjunto de datos incluye varias características sobre los pasajeros, como edad, sexo, clase y tarifa pagada. El objetivo es utilizar estos datos para construir un modelo predictivo que clasifique a los pasajeros como supervivientes o no supervivientes.

2. Propuesta de Solución
La solución al desafío del Titanic gira en torno al uso de modelos de aprendizaje automático supervisado. Los pasos principales incluyeron:

Análisis Exploratorio de Datos (EDA): Se utilizaron visualizaciones y resúmenes estadísticos para comprender las relaciones entre las variables y las tasas de supervivencia.
Ingeniería de Características: Se identificaron y transformaron características importantes (por ejemplo, manejo de valores faltantes, creación de nuevas características relevantes como el tamaño de la familia, codificación de variables categóricas).
Modelado: Se probaron y optimizaron una variedad de modelos, como Random Forest, Máquinas de Vectores de Soporte (SVM) y Regresión Logística, utilizando técnicas como validación cruzada y ajuste de hiperparámetros.

3. Desafíos Enfrentados
Datos Faltantes: Había valores faltantes en algunas características críticas como la edad y el lugar de embarque. Esto se abordó imputando los valores faltantes utilizando métodos estadísticos.
Conjunto de Datos Desequilibrado: El número de supervivientes y no supervivientes no estaba equilibrado, lo que conducía a posibles sesgos en el modelo. Se utilizaron técnicas como la validación cruzada estratificada y métricas apropiadas como ROC-AUC para manejar este problema. 
Escalado de Características: Dado que el conjunto de datos contenía características con diferentes escalas, se aplicó la normalización para garantizar que modelos como SVM funcionaran de manera óptima.

4. Soluciones a los Problemas
Datos Faltantes: Se realizó la imputación basándose en medianas para características numéricas y la categoría más frecuente para características categóricas.
Selección de Modelo: Se compararon varios modelos basándose en la precisión y las puntuaciones ROC-AUC. Se implementó el ajuste de hiperparámetros utilizando GridSearchCV para mejorar el rendimiento de los modelos seleccionados.
Validación Cruzada: Se utilizó la validación cruzada KFold para garantizar que el modelo se generalice bien a datos no vistos y evitar el sobreajuste.

5. Conclusión
El proyecto abordó con éxito el desafío del conjunto de datos del Titanic, ofreciendo información sobre qué factores contribuyeron más a la supervivencia y proporcionando un modelo bien optimizado que predice los resultados de supervivencia con sólidas métricas de rendimiento.

6. Tecnologías Utilizadas
Python (Pandas, NumPy, Scikit-learn)
Bibliotecas de Visualización (Matplotlib, Seaborn)
Técnicas de Aprendizaje Automático (Random Forest, SVM, Regresión Logística, PCA)
AWS S3 para el almacenamiento del conjunto de datos