# SVM vs Random Forest: Classification of forest cover types

## Descripción del proyecto

Este proyecto compara dos algoritmos de clasificación, Random Forest y Support Vector Machine (SVM), utilizando un dataset de clasificación multiclase. 
El objetivo principal es evaluar el rendimiento de ambos modelos y analizar sus fortalezas y debilidades en la predicción de diferentes clases.
El dataset proviene del UCI Machine Learning Repository y contiene información sobre diferentes tipos de cubiertas forestales. Las clases objetivo corresponden a distintos tipos de suelo.

## Objetivos
- Comprender el tratamiento de datos que hay que realizar para los modelos de clasificación.
- Entender y aplicar el algoritmo de Random Forest a un problema de clasificación.
- Entender y aplicar el algoritmo de Support Vector Machine (SVM) a un problema de clasificación.
- Evaluar y analizar los resultados de los clasificadores.

## Flujo de trabajo

- Preprocesamiento de datos:
  - Separación de datos
  - Distinción de variables
  - Normalización de variables continuas.
  - Balanceo del dataset.
  - Tratamiento de outliers.
- Entrenamiento de modelos:
  - Ajuste de hiperparámetros para Random Forest.
  - Ajuste de hiperparámetros para SVM.
- Evaluación de modelos:
  - Métricas de rendimiento en entrenamiento y test.
  - Análisis de matrices de confusión.
- Comparación y análisis:
  - Comparación de los mejores modelos de ambos algoritmos en términos de métricas globales y por clase.

## Resultados

| Modelo                 | Accuracy (Test) | Macro Precision | Macro Recall | Macro F1-Score | Observaciones                                                                 |
|------------------------|-----------------|-----------------|--------------|----------------|-------------------------------------------------------------------------------|
| **Random Forest (100 árboles)** | 68.62% | 59%            | 82%            | 64%           | Buen rendimiento en clases mayoritarias, pero dificultades en clases minoritarias. |
| **SVM (C=1000)**       | 85.53%          | 77%            | 80%            | 79%           | Mejor balance general, destacable en clases minoritarias aunque algo limitado por los datos. |

En general, SVM demostró un rendimiento superior, pero Random Forest puede ser más interpretativo y rápido para datasets grandes.

## Próximas mejoras

- Mejor búsqueda de hiperparámetros tanto para Random Forest como para SVM haciendo uso de GridSearch.
- Reducción de dimensionalidad:
  - Aplicar PCA para acelerar el entrenamiento de SVM sin perder mucha información.
- Probar con otras técnicas de escalado para SVM.
- Hacer uso de la validación cruzada.
