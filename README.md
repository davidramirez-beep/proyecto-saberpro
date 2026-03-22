# Proyecto Análisis de Datos - Saber Pro

## Descripción

Este proyecto tiene como objetivo realizar un análisis exploratorio de datos (EDA), junto con técnicas de preprocesamiento y reducción de dimensionalidad, utilizando el dataset de las pruebas Saber Pro en Colombia.

El trabajo se desarrolla como parte del curso de Análisis de Datos, aplicando conceptos como limpieza de datos, visualización, detección de patrones y transformación de variables.

---

##  Dataset

- Fuente: Datos de pruebas Saber Pro
- Tipo: Datos tabulares
- Formato: Excel (.xlsx)

El dataset contiene información académica, sociodemográfica y resultados de estudiantes en las pruebas Saber Pro.

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
│ └── SaberPro.xlsx
│
├── notebooks/
│ ├── 01_exploracion.ipynb
│ ├── 02_eda.ipynb
│ ├── 03_preprocesamiento.ipynb
│
├── README.md
├── requirements.txt

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