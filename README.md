# Proyecto Predicción de deserción estudiantil

## Miembros del grupo

* Karen Eliana Garcia Perez, Cc.1001296009, Ingeniría Civil

## Datos

Los datos del proyecto vienen de [kaggle](https://www.kaggle.com/datasets/thedevastator/higher-education-predictors-of-student-retention) y se pueden hacer disponibles realizando los siguientes pasos:

1. Crea una cuenta o inicia sesión en Kaggle 
2. Desde la parte superior derecha da click en tu foto de perfil
3. Sigue la ruta You profile/ Acount / API / Create new token
4. Guarda en tu ordenador el archivo que se descarga con el nombre kaggle.json
5. Ejecuta los siguientes comandos en el notbook
```
from google.colab import file
file.upload() #Cargar desde el ordenador el archivo kaggle.json

```
```
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
```

```
!kaggle datasets download -d thedevastator/higher-education-predictors-of-student-retention/
```

```
!unzip higher-education-predictors-of-student-retention.zip -d data
```
```
import pandas as pd
df = pd.read_csv('data/dataset.csv')
df.head()
```

## Videos
* [Video primera entrega](https://www.youtube.com)
* [Video segunda entrega](https://www.youtube.com)
