# Proyecto Análisis de Datos - Saber Pro

## Descripción

Este proyecto tiene como objetivo realizar un análisis exploratorio de datos (EDA), junto con técnicas de preprocesamiento y reducción de dimensionalidad, utilizando el dataset de las pruebas Saber Pro en Colombia.

El trabajo se desarrolla como parte del curso de Análisis de Datos, aplicando conceptos como limpieza de datos, visualización, detección de patrones y transformación de variables.

---

##  Dataset

1. Tabular
- Fuente: Datos abiertos Colombia
- Tipo: Tabular
- Origen : Secundaria (Este dataset proviene del ICFES y fue obtenido a través del portal Datos Abiertos Colombia.Es decir, los datos ya fueron recolectados por otra entidad.)

Características básicas
Número de registros (filas): 48.990
Número de variables (columnas): 58
Tamaño del archivo: 14 MB

Documentación y aplicaciones
Nivel de documentación:
El dataset cuenta con una descripción general en el portal Datos Abiertos Colombia, donde se explica su origen y propósito. Además, está relacionado con el ICFES.
Sin embargo, no incluye un diccionario de datos completamente detallado dentro del archivo, por lo que algunas variables pueden generar dudas.

Comprensión de variables:
Es un dataset de complejidad media:
Incluye variables claras como género, edad, institución educativa y puntajes por competencias
Contiene múltiples columnas relacionadas con resultados en módulos (lectura crítica, inglés, razonamiento cuantitativo, etc.)
Algunas variables tienen nombres técnicos o abreviados, lo que dificulta su interpretación sin documentación adicional

Aplicaciones:

Análisis educativo
Análisis socioeconómico
Visualización de datos (dashboards en Power BI o Python)
Modelos de Machine Learning para predicción de rendimiento académico
Proyectos académicos de análisis de datos


2. Texto
- Fuente : Kaggle
- Tipos de datos : Texto
- Origen : Secundaria (los datos fueron recolectados y publicados por terceros en la plataforma Kaggle)

Características básicas
Número de registros: 536
Número de variables: 2 (texto y categoría)
Distribución de clases:
Frutas: 176
Legumbres: 180
Verduras: 180
Tamaño del archivo: 4,32 KB

Documentación y aplicaciones
Nivel de documentación:
El dataset cuenta con una descripción general en Kaggle que explica su objetivo, aunque no incluye un diccionario de datos detallado.

Comprensión de variables:
Es un dataset sencillo y fácil de interpretar:
Una variable contiene el nombre del alimento (texto)
Otra variable indica la categoría (fruta, legumbre o verdura)

Aplicaciones:
Clasificación de texto
Procesamiento de lenguaje natural (NLP)
Entrenamiento de modelos de Machine Learning
Proyectos educativos de análisis de datos


3. Imágenes
Fuente: Kaggle
Tipo: Imágenes
Origen: Secundaria (Este dataset fue recopilado como parte de un proyecto académico de Machine Learning del Instituto Data Science y publicado en Kaggle, por lo que no fue recolectado directamente por el usuario.)

Características básicas
Número de registros (imágenes): 36 imágenes (una por año desde 1986 hasta 2021)
Número de variables (columnas): No aplica directamente (las imágenes contienen información en bandas espectrales como nir, swir1 y red)
Tamaño del archivo: 495 MB

Documentación y aplicaciones

Nivel de documentación:
El dataset cuenta con una descripción detallada en Kaggle, donde se explica el objetivo del proyecto, el contexto del análisis de deforestación y los archivos incluidos.
Además, incluye un informe del trabajo realizado, lo que mejora la comprensión general del dataset.

Comprensión de variables:
Es un dataset de complejidad media:

Las imágenes satelitales están en formato .tif y utilizan combinaciones de bandas (nir, swir1, red) para resaltar la vegetación
Incluye datasets adicionales en formato CSV como:
Datos de entrenamiento para modelos supervisados
Métricas del modelo
Series temporales de deforestación
Datos de error del modelo
Requiere conocimientos básicos de teledetección o análisis de imágenes para su correcta interpretación

Aplicaciones:

Análisis ambiental (deforestación)
Visión por computador (Computer Vision)
Modelos de Machine Learning supervisado
Análisis de series temporales
Proyectos académicos de ciencia de datos


Dataset seleccionado: SaberPro (ICFES)

El dataset seleccionado para el desarrollo del proyecto es el dataset tabular correspondiente a los resultados de las pruebas Saber Pro.

Justificación:
Completitud:
El dataset cuenta con un alto número de registros (48.990), lo que permite realizar un análisis robusto. Además, presenta posibles valores faltantes que pueden ser tratados en el análisis exploratorio.

Relevancia:
Los datos corresponden al contexto educativo en Colombia, lo que lo hace altamente relevante para el análisis socioeconómico y académico.

Documentación:
Aunque no cuenta con un diccionario de datos completamente detallado, el dataset incluye una descripción general en el portal de Datos Abiertos, lo que permite comprender su estructura y propósito.

Manejabilidad:
Al estar en formato tabular (Excel), es fácilmente manipulable mediante herramientas como Python (pandas) o Power BI, lo que facilita su análisis exploratorio y preprocesamiento.

---

## Objetivos

- Comprender la estructura y calidad de los datos
- Identificar valores faltantes y posibles outliers
- Analizar la distribución de variables
- Explorar relaciones entre variables
- Aplicar técnicas de preprocesamiento
- Reducir la dimensionalidad mediante PCA


---

##  Metodología

El proyecto se divide en tres fases principales:

###  1. Exploración de datos
- Revisión de estructura
- Tipos de datos
- Estadísticas descriptivas

###  2. Análisis Exploratorio (EDA)
- Identificación de valores faltantes
- Detección de outliers
- Análisis de distribuciones
- Correlaciones entre variables
- Visualizaciones (histogramas, boxplots, heatmaps)

###  3. Preprocesamiento
- Codificación de variables categóricas
- Escalado de variables numéricas
- Reducción de dimensionalidad (PCA)

---

##  Principales hallazgos

- Se identificaron valores atípicos en los puntajes de los estudiantes
- Existe una relación entre el estrato socioeconómico y el desempeño académico
- Se encontraron correlaciones entre variables académicas
- Algunas variables presentan valores faltantes que requieren tratamiento
- La reducción de dimensionalidad permitió simplificar la estructura del dataset

---

##  Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / VS Code

---

## 📁 Estructura del proyecto

proyecto-saberpro/
│
├── data/
│   ├── tabular/
│   │   └── SaberPro.xlsx
│   │
│   ├── texto/
│   │   ├── db-frutas.txt
│   │   ├── db-legumes.txt
│   │   └── db-verduras.txt
│   │
│   └── imagenes/
│       ├── raw/
│       │   ├── 2014-12-06.tif
│       │   ├── 2015-12-25.tif
│       │   ├── 2016-12-11.tif
│       │   ├── ...
│       │
│       └── processed/
│           ├── area_0.csv
│           ├── error_0.csv
│           ├── mean_data.csv
│           └── train_df.csv
│
├── README.md


## ▶️ Cómo ejecutar el proyecto

1. Clonar el repositorio:

git clone https://github.com/davidramirez-beep/proyecto-saberpro


2. Entrar al proyecto:

cd proyecto-saberpro


3. Crear entorno virtual:

python -m venv venv


4. Activar entorno:

Windows:

venv\Scripts\activate


5. Instalar dependencias:

pip install -r requirements.txt


6. Ejecutar notebooks desde VS Code o Jupyter

---

## 📌 Conclusiones

El análisis permitió comprender mejor la estructura de los datos de Saber Pro y detectar patrones relevantes en el desempeño de los estudiantes. 

El uso de técnicas de preprocesamiento y reducción de dimensionalidad facilita futuras etapas de modelado y análisis predictivo.

---

## 👥 Autores

- Andres Botero Bernal
- David Ramirez Velez

---

## 🎥 Video

Se incluye un video explicativo donde se presentan:
- Las bases de datos exploradas
- El proceso de análisis
- Principales hallazgos
- Conclusiones del proyecto