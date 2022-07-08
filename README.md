# Generación de Variables Climatológicas

[Jupyter Notebook](https://github.com/EddAngulo/generate_weather_variables/blob/main/src/generate_weather_variables.ipynb) desarrollado para generar diversas variables climatológicas (Humedad, Precipitación, Presión, Temperatura y Sensación Térmica).

## Dependencias
- [jupyter](https://jupyter.org/)
- [matplotlib](https://matplotlib.org/)
- [numpy](https://numpy.org/)
- [pandas](https://pandas.pydata.org/)
- [scikit-learn](https://scikit-learn.org/stable/)
- [seaborn](https://seaborn.pydata.org/)
- [xgboost](https://xgboost.readthedocs.io/en/stable/)

## Instalar dependencias
Para instalar las depedencias necesarias se debe usar `pip3 install -r requirements.txt` en el directorio del proyecto.

## Fuentes de datos
- [Humedad](https://www.datos.gov.co/Ambiente-y-Desarrollo-Sostenible/Humedad-del-Aire-2-metros/uext-mhny)
- [Precipitación](https://www.datos.gov.co/Ambiente-y-Desarrollo-Sostenible/Precipitaci-n/s54a-sgyg)
- [Presión](https://www.datos.gov.co/Ambiente-y-Desarrollo-Sostenible/Presi-n-Atmosf-rica/62tk-nxj5)
- [Temperatura](https://www.datos.gov.co/Ambiente-y-Desarrollo-Sostenible/Datos-Hidrometeorol-gicos-Crudos-Red-de-Estaciones/sbwg-7ju4)

Los archivos `.csv` de cada variable se deben guardar en el directorio correspondiente especificado en el Notebook. Estos directorios se generan automáticamente al ejecutar la sección `Creación del Árbol de Directorios` en el Notebook.

## Estructura de los datos
Todos los datasets (archivos `.csv`) de las variables previamente mencionadas están compuestos por las siguientes columnas:
- `CodigoEstacion`
- `CodigoSensor`
- `FechaObservacion`
- `ValorObservado`
- `NombreEstacion`
- `Departamento`
- `Municipio`
- `ZonaHidrografica`
- `Latitud`
- `Longitud`
- `DescripcionSensor`
- `UnidadMedida`

En el desarrollo del notebook solo se tomaron en consideración las columnas `FechaObservacion`, `ValorObservado` y `Departamento`.

# Merge Datasets

[Jupyter Notebook](https://github.com/EddAngulo/generate_weather_variables/blob/main/src/merge_datasets.ipynb) desarrollado unir los distintos datasets en uno solo.

## Dependencias
- [holidays](https://pypi.org/project/holidays/)
- [jupyter](https://jupyter.org/)
- [numpy](https://numpy.org/)
- [pandas](https://pandas.pydata.org/)
- [xlrd](https://xlrd.readthedocs.io/en/latest/)

## Instalar dependencias
Para instalar las depedencias necesarias se debe usar `pip3 install -r requirements.txt` en el directorio del proyecto.

## Datasets
Los archivos `.csv` y `.xlsx` se deben guardar en el directorio correspondiente especificado en el Notebook. Estos directorios se generan automáticamente al ejecutar la sección `Creación del Árbol de Directorios` en el Notebook.