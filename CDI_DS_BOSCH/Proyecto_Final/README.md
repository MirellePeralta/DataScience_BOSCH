# Clasificación de Casos de COVID-19 - Proyecto de Data Science

Este proyecto se centra en analizar y clasificar casos de COVID-19 utilizando técnicas de Data Science. El objetivo principal es construir modelos de clasificación para predecir la clasificación final de los casos.

## Conjunto de Datos

El conjunto de datos utilizado se obtuvo de [Datos Abiertos sobre COVID-19 en México](https://datos.gob.mx/busca/dataset/informacion-referente-a-casos-covid-19-en-mexico). Contiene información detallada sobre casos de COVID-19, incluyendo diversas variables como sexo, edad, comorbilidades y resultados de pruebas.

## Preprocesamiento de Datos

Antes de aplicar modelos de clasificación, se realizaron varias operaciones de preprocesamiento:

- Eliminación de registros no relevantes.
- Eliminación de columnas no influyentes para el análisis.
- Manejo de valores nulos y ajuste de formatos de fecha.

## Exploración de Datos

Se realizaron análisis descriptivos para comprender mejor la distribución de las variables y su impacto en la clasificación final de casos de COVID-19.

## Modelo de Clasificación

### Random Forest Classifier

Se utilizó el algoritmo de Bosques Aleatorios para construir un modelo de clasificación. Se entrenó el modelo utilizando datos de entrenamiento y se evaluó su rendimiento en datos de prueba.

| Clase | Precisión | Recall | F1-Score | Soporte |
|-------|-----------|--------|----------|---------|
| 1     | 0.15      | 0.04   | 0.06     | 3951    |
| 3     | 1.00      | 1.00   | 1.00     | 209997  |
| 6     | 0.97      | 0.98   | 0.97     | 32301   |
| 7     | 0.99      | 1.00   | 0.99     | 345915  |

**Precisión Global (Accuracy):** 0.9907

**Promedio Ponderado (Weighted Avg):** 0.99


## Interfaz de Usuario Interactiva

Se implementó una interfaz de usuario interactiva utilizando Gradio para permitir a los usuarios realizar predicciones sobre nuevos casos de COVID-19 basándose en los modelos entrenados.
