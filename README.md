# 🏠 Predicción de precios de Airbnb – Machine Learning

## 📌 Objetivo del proyecto
El objetivo de esta práctica es abordar un **problema realista de Machine Learning** siguiendo una metodología correcta y buenas prácticas vistas en clase.  
En concreto, se trata de un **problema de regresión**, cuyo fin es **predecir el precio de un alojamiento de Airbnb** a partir de las variables disponibles en el dataset.

Más allá de obtener un buen resultado numérico, el foco principal del proyecto está en:
- La **calidad del proceso seguido**
- La **correcta preparación de los datos**
- La **elección razonada de modelos y métricas**



## 📊 Conjunto de datos
El dataset utilizado procede de **Airbnb** y ha sido obtenido mediante técnicas de *web scraping*.  
Se trata de **datos reales**, por lo que contiene:
- Valores nulos
- Variables categóricas
- Outliers
- Posibles problemas de correlación entre variables

Esto hace necesario un análisis y limpieza de datos más cuidadosos que en datasets sintéticos.



## 🧠 Metodología seguida

El proyecto se ha desarrollado de forma **incremental**, comenzando por soluciones sencillas y aumentando progresivamente la complejidad.

### 1️⃣ Preparación de los datos
- División del dataset en **train** y **test**
- Separación de la variable objetivo (*price*)

### 2️⃣ Análisis exploratorio de datos (EDA)
- Inspección inicial: `head()`, `describe()`, `info()`, tipos de datos
- Análisis de valores nulos
- Estudio de **outliers**
- Análisis de **correlación** entre variables
- Visualización mediante histogramas y matrices de correlación

### 3️⃣ Preprocesamiento
- Eliminación de variables:
  - Con alto porcentaje de valores nulos
  - Poco informativas (IDs, texto irrelevante)
  - Altamente correlacionadas
- Transformación de variables categóricas:
  - *One-Hot Encoding*
  - *Target Encoding*
- Imputación de valores nulos
- Escalado de variables numéricas cuando el modelo lo requiere

### 4️⃣ Selección de variables
- Uso de modelos como **Random Forest** para analizar la importancia de las variables
- Selección de las variables más relevantes para el modelado final

### 5️⃣ Modelado
- Entrenamiento de distintos modelos de regresión
- Uso de **cross-validation**
- Comparación de resultados entre modelos

### 6️⃣ Evaluación
- Evaluación del rendimiento en conjunto de test
- Métricas utilizadas:
  - MSE
  - R²
  - RMSE
- Comparación entre modelos para seleccionar el más adecuado



## 📈 Resultados
Los resultados obtenidos son **razonables**, teniendo en cuenta la complejidad y la naturaleza real del dataset.  
El énfasis del proyecto no está en maximizar la métrica, sino en garantizar:
- Un pipeline coherente
- Ausencia de errores conceptuales
- Correcta separación entre train y test



## 📝 Conclusiones
Este proyecto demuestra cómo abordar un problema real de Machine Learning de forma estructurada, desde el análisis exploratorio hasta la evaluación del modelo.  
La práctica pone de manifiesto la importancia de la **limpieza de datos**, la **selección de variables** y la **comparación de modelos**, más allá de la métrica final obtenida.



## 🛠️ Tecnologías utilizadas
- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn
- Jupyter Notebook

