# Actividad Integradora #3:

Clasificador de Animales

Equipo 3: 

- Héctor Noel	A01251806
- Fernando	A00819824
- Ricardo Marcelo	A01176405
- Alitzel Adriana	A01373166
- Adrián Ricardo	A01196967

Contenido:

**Data_Collection_Script.py**: 

Archivo que se encarga de descargar las imagenes de Shutterstock utilizando la librería de selenium webdriver. 
Se le pide un término de busuqueda al usuario y a partir de este se buscan las imagenes. Se dividen en particiones de 70 20 10.

**Vgg16_classifier.ipynb**:

Archivo principal donde se crea y construye el clasificador de arquitectura Vgg16. Se divide en las siguientes secciones:

- Data augmentation

Obtiene las imagenes del directorio predeterminado 'train' y genera variaciones de los datos existentes mediante la función 
ImageDataGenerator() con rotaciones, shifting, zooming, y flipping. Después de que se genere, se grafican las imagenes.

- Recoleccion y procesamiento de datos

Esta seccion se divide entre el conjunto de entrenamiento, el conjunto de pruba y el conjunto de validación. 
Para cada uno de estos conjuntos se grafíca que tantas imagenes pertenecen a que clases.

- Selección y entrenamiento de modelos

Esta sección es la sección principal del documento, que construye el modelo utilizando la libreria keras y la información proporcionada anteriormente.


Como ejecutar:

Primero, ejecute el sript Data_Collection_Script.py en un directorio donde se puedan almacenar las imagenes, para descargar las imagenes. 
Después, en Jupyter abra el archivo Vgg16_classifier.ipynb y ejecute una por una las celdas para ver el proceso de construcción del clasificador vgg16.

Nota:

- El conjunto de imagenes usado para entrenar este modelo puede ser encontrado en el siguiente link:
[Descargar imagenes](https://drive.google.com/drive/folders/1P8oQyOtKx_Lt18WH-dHzTVUn4xBh9F5d?usp=sharing)

Para ejecutar en Google Colab:

1) descargar los folders 'train', 'test' y 'validation' individualmente como zips.
2) subir los zips a Google colab
3) ejecutar los imports en la seccion 'Selección y entrenamiento de modelos'
4) ejecutar los comandos !unzip en la seccion de 'Recoleccion y procesamiento de datos
5) ejecutar el resto de las celdas y ver los resultados.

[link al colab](https://drive.google.com/file/d/1TvAYvAX2lS2uMC2mujeCabBs94Sa9F38/view?usp=sharing)