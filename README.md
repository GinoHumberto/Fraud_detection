# Detección de Fraude Bancario

Trabajo Final Integrador de la **Diplomatura en Ciencia de Datos y Análisis Avanzado — UTN**.

## Descripción

El proyecto consiste en desarrollar un sistema de detección de transacciones bancarias fraudulentas utilizando técnicas de Machine Learning y Deep Learning.

Se utiliza el dataset sintético **BankSim**, con el objetivo de identificar operaciones potencialmente fraudulentas y priorizar las investigaciones, minimizando las falsas alarmas.

## Metodología

El desarrollo incluye:

- Análisis exploratorio y limpieza de datos.
- Ingeniería de variables históricas de clientes, comercios y categorías.
- División temporal en entrenamiento, validación y prueba.
- Comparación de modelos con y sin ingeniería de variables.
- Evaluación mediante Average Precision, ROC-AUC y Card Precision@20.

### Modelos evaluados

- Regresión Logística
- Random Forest
- XGBoost
- Red neuronal Feedforward (Keras)

## Resultados

El mejor modelo fue la **red neuronal Feedforward con ingeniería de variables**, obteniendo los siguientes resultados sobre el conjunto de prueba:

| Métrica | Resultado |
|---|---|
| Average Precision | 0.8800 |
| ROC-AUC | 0.9993 |
| Card Precision@20 | 0.2239 |

## Tecnologías

Python · Pandas · NumPy · Scikit-learn · XGBoost · TensorFlow/Keras · Matplotlib · Seaborn

## Dataset y referencias

- [BankSim — Kaggle](https://www.kaggle.com/datasets/ealaxi/banksim1)
- [Fraud Detection Handbook](https://fraud-detection-handbook.github.io/fraud-detection-handbook/)

## Ejecución

1. Instalar las dependencias del proyecto.
2. Descargar el dataset BankSim y ubicarlo en la carpeta `Dataset/`.
3. Abrir y ejecutar el notebook `Trabajo_final.ipynb`.

**Nota:** El proyecto utiliza datos sintéticos y sus resultados no representan una validación sobre transacciones bancarias reales.