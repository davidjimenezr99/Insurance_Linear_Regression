# Análisis y Modelo Predictivo del Insurance Dataset

Este proyecto realiza un análisis exploratorio y predictivo utilizando el **dataset `insurance`**. El objetivo principal fue modelar la relación entre diversas características de los clientes y los cargos médicos (`charges`) utilizando **regresión lineal**. Se examinaron los principales supuestos de la regresión lineal (multicolinealidad, heterocedasticidad, normalidad e independencia de los residuos) para asegurar la validez del modelo. Además, se experimentó con técnicas de regularización como **Ridge** y **Lasso** para mejorar el ajuste del modelo.

## Archivos en el Repositorio

- **insurance.csv**: Archivo de datos con información de clientes y sus cargos médicos.
- **linear_regression_model.pkl**: Archivo que contiene el modelo de regresión lineal entrenado.
- **Insurance_linear_regression.ipynb**: Jupyter Notebook que contiene el análisis exploratorio, pruebas de multicolinealidad, heterocedasticidad, normalidad e independencia de los residuos, así como la creación y evaluación de los modelos de **regresión lineal**, **Ridge** y **Lasso**.

## Requisitos

Para ejecutar el código y reproducir el análisis, necesitarás las siguientes bibliotecas:

- `pandas`
- `numpy`
- `scikit-learn`
- `scipy`
- `statsmodels`
- `matplotlib` (opcional, para visualizaciones)
- `joblib` (para guardar y cargar los modelos)

## Modelo y Evaluación

Se entrenó un modelo de **regresión lineal** para predecir los cargos médicos (`charges`). Para asegurar la calidad del modelo, se realizaron las siguientes pruebas:

1. **Multicolinealidad**: Mediante el cálculo de la **matriz de correlación**
2. **Heterocedasticidad**: Se utilizó la **prueba de Breusch-Pagan** para verificar si la varianza de los residuos es constante.
3. **Normalidad**: Se aplicó la **prueba de Shapiro-Wilk** para verificar si los residuos seguían una distribución normal.
4. **Independencia**: Se utilizó el **test de Durbin-Watson** para asegurar que los residuos no estuvieran autocorrelacionados.

### Técnicas adicionales:

- **Ridge** y **Lasso**: Se entrenaron modelos con regularización para evaluar si mejoraban la predicción y reducían el sobreajuste. Sin embargo, el mejor modelo fue el de **regresión lineal simple**
### Evaluación:

## Referencias

Dataset: **Insurance Charges Dataset** (disponible en plataformas como Kaggle o repositorios de ejemplos de `scikit-learn`).
