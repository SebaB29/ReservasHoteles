# 🏨 ReservasHoteles  
**Trabajo Práctico para la materia Organización de Datos (95.58)**

## 👥 Integrantes  
| Nombre                      | Github                                   |
|-----------------------------|------------------------------------------|
| Sebastián Brizuela          | [SebaB29](https://github.com/SebaB29)    |
| Lucia Agha Zadeh Dehdeh     | [Lucia-azd](https://github.com/Lucia-azd)|
| Juan Sebastián Del Río      | [S2JuanS2](https://github.com/S2JuanS2)  |

## 📜 Descripción  
Competencia de Kaggle que consiste en obtener una predicción sobre si una reserva de hotel será cancelada o no.

<p align="justify">
Se realizó un análisis exploratorio de los datos de muestra (<i>CHP1</i>) utilizando herramientas proporcionadas por las librerías: <b>Pandas</b>, <b>Matplotlib</b>, <b>Seaborn</b>, <b>Numpy</b> y <b>Scipy</b>, además de un archivo con información sobre los datos proporcionado por la Cátedra.
</p>

### 🔍 Modelos Predictivos Utilizados  
Se exploraron distintos modelos predictivos para practicar su utilización:
* **DecisionTreeClassifier**
* **RandomForestClassifier**
* **KNeighborsClassifier**
* **SVC**
* **XGB**
* **VotingClassifier**
* **StackingClassifier**
* **Redes Neuronales**

## 📜 Enunciado
<p align="justify">
Los conjuntos de datos a utilizar, <i>hotels_train</i> y <i>hotels_test</i>, se encuentran disponibles en la competencia de Kaggle y deberán descargarlos desde allí. Allí mismo encontrarán un archivo de ejemplo de cómo se deben subir las soluciones.
Se deberán explorar los datos de train, realizar ingeniería de características y entrenar modelos de clasificación para poder predecir si una reserva será cancelada: el target será la variable <i>is_canceled</i>. Las tareas de preprocesamiento deberán replicarse en los datos de test, ya que será necesario obtener las predicciones sobre el conjunto de evaluación y subirlas a Kaggle.
</p>

### Etapas a Desarrollar  
1. **Análisis Exploratorio y Preprocesamiento de Datos**
   - Exploración Inicial
   - Visualización de los datos
   - Análisis de Datos Faltantes
   - Detección de Valores Atípicos

2. **Clasificación - Entrenamiento y Predicción**
   - Árbol de decisión
   - Modelos de ensamble (KNN, SVC, RF, XGBoost)
   - Redes Neuronales

## 📊 Reporte Final  

### Introducción

<p align="justify">
Se realizó un análisis exploratorio sobre un dataset de reservas de hoteles, que tiene 31 columnas y 61,913 filas. A través de análisis y visualizaciones, se determinaron las variables relevantes. Luego se pasó al preprocesamiento de datos, donde se detectaron columnas con datos faltantes y outliers, a los cuales se les aplicó su correspondiente tratamiento. Se exploraron distintos modelos de clasificación en la búsqueda de mejores métricas para predecir si la reserva fue cancelada o no.
</p>

### Cuadro de Resultados  
| CHP | Modelo             | F1 Score | Precision Test | Recall Test | Accuracy | Kaggle   |
|-----|--------------------|----------|----------------|-------------|----------|----------|
| 2   | Árbol              | 0.85184  | 0.84518        | 0.83861     | 0.84570  | 0.84082  |
| 3   | Stacking (Mejor)   | 0.86116  | 0.86498        | 0.86884     | 0.86379  | 0.86193  |
| 4   | Red Neuronal       | 0.82974  | 0.76997        | 0.89957     | 0.81459  | 0.80829  |

### Conclusiones Generales
<p align="justify">
A partir del análisis exploratorio realizado en el dataset de reservas de hoteles, se han obtenido diversas conclusiones. En primer lugar, se realizó un análisis de los datos que incluyó un preprocesamiento que aportó una buena base para obtener buenas predicciones, incluyendo la gestión de datos faltantes y la identificación y tratamiento de valores atípicos. 
</p>

- En términos de simplicidad y velocidad de entrenamiento, **XGBoost** se destacó como el modelo más sencillo y rápido de entrenar, obteniendo el segundo mejor resultado en Kaggle.
- El modelo **Stacking** demostró ser el más efectivo en la competencia de Kaggle.

<p align="justify">
En resumen, el análisis exploratorio y las decisiones tomadas en el preprocesamiento fueron fundamentales para mejorar las predicciones de los modelos. Aunque consideramos que nuestros modelos son buenos para ser los primeros que realizamos, es importante seguir explorando y experimentando con diferentes enfoques para lograr mejoras en la performance predictiva de nuestros modelos.
</p>

## 📄 Licencia  
Este proyecto está bajo la licencia MIT. Para más detalles, consulta el archivo [LICENSE](./LICENSE).
