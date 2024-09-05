# Clasificación del Estado de Colmenas mediante Machine Learning

Este repositorio contiene el código, datos y recursos utilizados en el estudio "Machine Learning en la Apicultura: Clasificación Avanzada del Estado de Colmenas con Pipeline Optimizado y Etiquetado Preciso" por Axel A. Skrauba, Hector De Sosa, y Sandro D. Zakowicz.

## Descripción del Proyecto

Este proyecto aplica técnicas avanzadas de machine learning para clasificar el estado de colmenas de abejas (Apis Mellifera) basándose en el análisis de audio del zumbido de la colmena. El estudio se centra en la identificación de cuatro estados diferentes relacionados con la presencia y aceptación de la reina en la colmena.

## Estructura del Repositorio
```
├── data/
│   ├── raw/                 # Datos de audio sin procesar, link a repositorio oficial
│   ├── processed/           # Datos procesados y características extraídas
│   └── metadata.csv         # Metadatos de las grabaciones, originales del repositorio oficial
├── notebooks/
│   ├── 1_data_exploration.ipynb
│   ├── 2_feature_extraction.ipynb
│   ├── 3_model_training.ipynb
│   ├── 4_label_correction.ipynb
│   └── 5_pipeline_optimization.ipynb
├── models/
│   └── best_model.pkl       # Modelo entrenado con mejor rendimiento
├── results/
│   ├── figures/             # Gráficos y visualizaciones generadas
│   └── metrics.csv          # Métricas de rendimiento de los modelos
├── requirements_pycaret.txt # Dependencias para PyCaret
├── requirements_cleanlb.txt # Dependencias para CleanLab
└── Articulo BeeHive.pdf     # Documento pdf en formato de artículo, con el desarrollo del proyecto
└── README.md                # Este archivo
```
## Instalación y Uso

1. Se sugiere la utilización de un entorno virtual dedicado para cada etapa (virtualenv, por ejemplo)
2. Clonar el repositorio desde GitHub.
3. Instalar las dependencias necesarias según su objetivo, ejemplo utilizando `pip install -r requirements_pycaret.txt`.
4. Explore los notebooks en el directorio `notebooks/` para ver el flujo de trabajo completo.

## Datasets

El conjunto de datos utilizado en este estudio proviene del Smart Bee Colony Monitor Dataset, disponible públicamente en [Kaggle](https://www.kaggle.com/datasets/annajyang/beehive-sounds/data). Una mejor descripción de los audios originales se encuentra en el directorio `data/raw/`.

## Notebooks

1. `1_data_exploration.ipynb`: Análisis exploratorio de los datos de audio y visualización de espectrogramas.
2. `2_feature_extraction.ipynb`: Extracción de características MFCC de los archivos de audio.
3. `3_model_training.ipynb`: Entrenamiento y evaluación de modelos de clasificación iniciales.
4. `4_label_correction.ipynb`: Implementación de Cleanlab para la corrección de etiquetas.
5. `5_pipeline_optimization.ipynb`: Pipeline de procesamiento y entrenamiento con etiquetas corregidas.

## Modelos

El modelo con mejor rendimiento (CatBoost Classifier) se encuentra guardado en `models/best_model.pkl`.

## Resultados
Los resultados detallados, incluyendo métricas de rendimiento y visualizaciones, se encuentran en el directorio `results/`.
Para una descripción contextualizada acceda al [Artículo](https://github.com/AxelSkrauba/queen-bee-status/blob/main/Articulo%20BeeHive.pdf).

## Contribuciones
Las contribuciones son bienvenidas. Por favor, abra un issue para discutir cambios importantes antes de crear un pull request.
