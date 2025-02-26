# Análisis y Predicción del Precio de Acciones de NVIDIA

Este proyecto utiliza Python y bibliotecas de machine learning para analizar y predecir el precio de las acciones de NVIDIA (NVDA) mediante un modelo de regresión lineal.

## Características Principales
- 🚀 **Carga y preprocesamiento de datos** desde un archivo CSV.
- 📊 **Visualización de datos** usando `matplotlib` y `mplfinance`.
- 🏗️ **Ingeniería de Características** con `OneHotEncoder`.
- 🤖 **Entrenamiento del modelo de regresión lineal** con `scikit-learn`.
- 📈 **Evaluación del modelo** usando `mean_squared_error` y `r2_score`.
- 💾 **Guardado del modelo entrenado** con `pickle`.

## Requisitos
Asegúrese de tener instaladas las siguientes bibliotecas antes de ejecutar el notebook:

```bash
pip install pandas matplotlib seaborn mplfinance scikit-learn
```

## Uso
1. 📂 **Carga de datos:**
   - El notebook lee un archivo `nvda.csv` que contiene los precios de las acciones de NVIDIA.
   - La columna de fecha se convierte en `datetime` y se establece como índice.
2. 📉 **Visualización:**
   - Se generan gráficos de velas para analizar las tendencias del mercado.
3. 🎯 **Entrenamiento del modelo:**
   - Se separan las variables `Open`, `High`, `Low` y `Adj Close`.
   - Se codifican características categóricas (si las hay) y se divide el dataset en `train` y `test`.
   - Se entrena un modelo de regresión lineal.
4. 🔍 **Evaluación y Predicción:**
   - Se visualizan los resultados con `seaborn`.
   - Se guarda el modelo entrenado en `nvda_model.pkl`.

## Ejecución
Para ejecutar el notebook, simplemente abra:

```bash
jupyter notebook nvda_lr.ipynb
```

## Resultados
- 🏆 **Precisión del Modelo:** El modelo alcanzó una precisión de **0.9999988920659469** en el conjunto de prueba.

## Producción
Si deseas probar el modelo en producción, puedes hacerlo desde el siguiente repositorio: [https://github.com/0xfabrica/nvda_lr](https://github.com/0xfabrica/nvda_lr).

## Autor
Este proyecto fue desarrollado en un entorno de Google Colab y posteriormente convertido en un notebook para su ejecución local. Cualquier mejora o retroalimentación es bienvenida.
