# Datos Crudos del Smart Bee Colony Monitor Dataset

Este directorio está destinado a contener los datos de audio sin procesar utilizados en nuestro estudio sobre la clasificación del estado de colmenas mediante machine learning. Sin embargo, debido al tamaño de los archivos y a consideraciones de derechos de autor, los datos no se incluyen directamente en este repositorio.

## Descripción del Dataset

El Smart Bee Colony Monitor Dataset contiene grabaciones de audio de colmenas de abejas (Apis Mellifera) en varios estados, incluyendo:

1. Reina original presente
2. Reina no presente
3. Reina presente pero rechazada
4. Reina presente y recién aceptada

Cada grabación es un segmento de audio de 60 segundos, muestreado a una frecuencia específica (consultar la documentación original para detalles técnicos precisos).

## Origen de los Datos

Los datos fueron recopilados y publicados originalmente por Anna Yang et al. como parte del proyecto Smart Bee Colony Monitor.

## Cómo Obtener los Datos

Para acceder a los datos crudos, siga estos pasos:

1. Visite la página del dataset en Kaggle: [Smart Bee Colony Monitor: Clips of Beehive Sounds](https://www.kaggle.com/datasets/annajyang/beehive-sounds)
2. Si aún no tiene una cuenta en Kaggle, necesitará crear una (es gratuito).
3. Una vez en la página del dataset, haga clic en el botón "Download" para descargar el archivo zip que contiene todos los datos.
4. Descomprima el archivo descargado y coloque los archivos de audio (.wav) en este directorio (data/raw/).

## Estructura de los Datos

Una vez descargados, los datos deben organizarse de la siguiente manera en este directorio:

```
data/raw/
├── sound_files/
│   ├── file1.wav
│   ├── file2.wav
│   └── ...
└── all_data_updated.csv
```

El archivo metadata.csv contiene información adicional sobre cada grabación, incluyendo la fecha, hora, ubicación, variables climáticas y el estado de la reina.

## Uso de los Datos

Asegúrese de citar adecuadamente la fuente original de los datos en cualquier publicación o proyecto que utilice este dataset. Consulte el archivo LICENSE en la raíz de este repositorio para obtener información sobre los términos de uso. A la fecha, es CC0 1.0 UNIVERSAL.

## Nota Importante

Antes de utilizar estos datos, asegúrese de leer y comprender los términos de uso y la licencia proporcionados por los autores originales en la página de Kaggle del dataset.
