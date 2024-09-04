# Datos Procesados

Este directorio está destinado a contener los datos de audio procesados. Se realizaron diversas pruebas.
En general, los archivos contienen las características resultantes de 50 MFCCs sobre los audios.
Se detallan las características, nombre del audio procesado ("file name") y etiqueta de salida ("label").

## Descripción de los Archivos

### Originales

* `output_file_50mfcc_4000Hz.csv` contiene el conjunto separado para TRAIN.
* `testoutput_file_50mfcc_4000Hz.csv` contiene el conjunto separado para TEST.

### Etiquetas limpias (usando un modelo base sobre 13 MFCC)
A fines de corroborar las etiquetas corregidas (limpias), las mismas se agregan como "label_updated".

* `output_file_50mfcc_4000Hz_CLEAN.csv` contiene el conjunto separado para TRAIN.
* `testoutput_file_50mfcc_4000Hz_CLEAN.csv` contiene el conjunto separado para TEST.

### Etiquetas limpias (usando un modelo base sobre 50 MFCC)

* `output_file_50mfcc_4000Hz_CLEANby50MFCC.csv` contiene el conjunto separado para TRAIN.
* `testoutput_file_50mfcc_4000Hz_CLEANby50MFCC.csv` contiene el conjunto separado para TEST.
