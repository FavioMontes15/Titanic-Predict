# 🚢 Titanic Predict

## 📌 Descripcion General del Proyecto

En este proyecto se analiza el dataset del Titanic para predecir la supervivencia de los pasajeros mediante mutiples modelos de clasificacion de machine learning. Realizamos un analisis exploratorio de datos para luego aplicar algoritmos de clasificación y evaluación de métricas.

## 📂 Dataset

- `Titanic.csv`
- Dataset importado del Seaborn

## ⚙️ Herramientas

- **Lenguajes:** Python, Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn, Plotly
- **Machine Learning:** Logistic Regression, SVM, KNN, Random Forest, Decision Tree
- **Otras herramientas:** Dash para la visualizacion

## 🔍 Preprocesamiento

- Eliminacion de columnas con exceso de valores faltantes
- Manejo de valores faltantes
- Codificacion de variables categóricas
- Normalizacion de variables numéricas

## 📊 Analisis Exploratorio de Datos (EDA)

- Graficos de conteo para la distribucion de supervivencia
- Histogramas para la distribucion de las edades
- Diagramas de caja para visualizar outliers en variables numéricas
- Graficos de contero para los puertos de embarque

## 🚀 Entrenamiento del modelo y evaluación

Los modelos fueron entrenados usando Pipelines:

1. **Preprocesamiento** (Escalado y codificado) (StandardScaler & OneHotEncoder)
2. **Division de datos** (80% train & 20% test) (train_test_split)
3. **Entrenamiento del modelo**(LR, KNN, Random Forest, SVM, Decision Tree)
4. **Ajuste de hiperparametros** (GridSearchCV para RandomForest)
5. **Metricas de evaluación para clasificación**
   - Accuracy
   - Precision
   - Recall
   - F1 Score
   - Cross-validation
   - Confusion Matrix

## 🔥 Seleccion del mejor modelo

El modelo mas optimo fue **Random Forest**, con un accuracy de 0.81 y una media CV de 0.828.

Ajustando los hiperparámetros del **Random Forest**, obtenemos un accuracy de 0.81 y una media CV de 0.822.

Si bien los valores del Random Forest sin ajustar y el Random Forest optimizado son parecidos, el modelo optimizado generaliza mejor en promedio a pesar que su score en el test sea un poco menor al score del modelo no optimizado.

