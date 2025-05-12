# Predicción de Riesgo de Hipertensión Basada en Hábitos Nutricionales con Machine Learning

Este repositorio contiene el código desarrollado para un Trabajo de Fin de Máster (TFM) enfocado en la predicción del riesgo de hipertensión a partir de datos demográficos y hábitos nutricionales, utilizando técnicas de Machine Learning, análisis explicativo y productivización del modelo.

## Descripción del Proyecto

El objetivo principal de este proyecto es construir un sistema inteligente capaz de predecir la probabilidad de hipertensión en individuos, utilizando para ello datos del estudio NHANES (National Health and Nutrition Examination Survey). Se implementan distintos modelos de aprendizaje supervisado, se aplican técnicas de balanceo de clases (SMOTE), selección de variables y se emplean herramientas de interpretabilidad para obtener modelos explicables.

## Modelos Implementados

Se entrenan y evalúan diversos modelos de clasificación binaria, incluyendo:

- Random Forest
- XGBoost
- LightGBM
- Gradient Boosting
- SVM (Support Vector Machines)
- Regresión Logística (con y sin selección de variables)

Los modelos se comparan en base a métricas como Accuracy, Precision, Recall, F1-Score y AUC-ROC.

## Tecnologías y Librerías Utilizadas

- Python 3.x
- pandas, numpy
- scikit-learn
- xgboost
- lightgbm
- seaborn, matplotlib
- shap (para interpretabilidad)
- Flask (para productivización del modelo)
- joblib (para serialización de modelos)

## Interpretabilidad

Se utiliza SHAP para analizar la importancia de las variables en los modelos entrenados, especialmente sobre la regresión logística con selección de características, lo que permite obtener interpretaciones claras y transparentes sobre los factores de riesgo.

## API de Predicción

Como parte de la productivización, se crea una API con Flask que permite cargar modelos previamente entrenados, escalar los datos de entrada y devolver predicciones para nuevos registros.


## Resultados Destacados

El mejor rendimiento se obtuvo con el modelo **SVM**, alcanzando una precisión de 0.99 y un AUC-ROC de 0.998 en un entorno balanceado. También se destaca la interpretabilidad ofrecida por la regresión logística con SHAP.


**Autor:** [Juan Diego Díaz Domínguez]  
**Contacto:** [www.linkedin.com/in/juan-diego-diaz-dominguez-52480b209]


