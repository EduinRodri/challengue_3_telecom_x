📊 Predicción de Cancelación de Clientes con Machine Learning

Este proyecto tiene como objetivo desarrollar modelos predictivos capaces de identificar qué clientes tienen mayor probabilidad de cancelar sus servicios (Customer Churn).

La cancelación de clientes representa un problema importante para las empresas de telecomunicaciones, ya que la pérdida de clientes impacta directamente en los ingresos. Por esta razón, mediante técnicas de Machine Learning, se busca anticipar este comportamiento y apoyar la toma de decisiones estratégicas orientadas a la retención de clientes.

El proyecto consiste en la construcción de un pipeline de análisis y modelado, que incluye la preparación de los datos, el entrenamiento de modelos de clasificación y la evaluación de su rendimiento.

🎯 Objetivos del desafío

Durante el desarrollo del proyecto se trabajó en los siguientes objetivos:

Preparar los datos para el modelado, incluyendo limpieza, tratamiento, codificación y normalización.

Realizar análisis de correlación entre variables para identificar relaciones relevantes.

Seleccionar variables que aporten mayor información para el modelo.

Entrenar dos o más modelos de clasificación para predecir la cancelación de clientes.

Evaluar el rendimiento de los modelos utilizando diferentes métricas.

Interpretar los resultados obtenidos, incluyendo la importancia de las variables.

Elaborar una conclusión estratégica identificando los principales factores que influyen en la cancelación.

🧠 Habilidades aplicadas

Durante el desarrollo de este proyecto se aplicaron y reforzaron las siguientes habilidades:

Preprocesamiento de datos para Machine Learning.

Construcción y evaluación de modelos predictivos.

Interpretación de resultados obtenidos a partir de modelos de clasificación.

Comunicación técnica de resultados con enfoque estratégico.

🧰 Tecnologías utilizadas

Para el desarrollo del proyecto se utilizaron las siguientes herramientas y librerías:

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Imbalanced-learn (SMOTE)

Estas herramientas permitieron realizar el análisis de datos, la visualización de información y la construcción de modelos de Machine Learning.

📁 Estructura del proyecto

El repositorio contiene los siguientes archivos principales:

cancelacion_clientes_machine_learning/

├── Telecom_X_2.ipynb
├── telecomx_churn_limpio.csv
├── requirements.txt
└── README.md
Descripción de los archivos

Telecom_X_2.ipynb
Notebook que contiene todo el proceso de análisis de datos, preprocesamiento, entrenamiento de modelos y evaluación de resultados.

telecomx_churn_limpio.csv
Dataset utilizado para el análisis y entrenamiento de los modelos.

requirements.txt
Archivo que contiene las librerías necesarias para ejecutar el proyecto.

README.md
Documento de descripción general del proyecto.

⚙️ Instalación del proyecto

Para ejecutar este proyecto en un entorno local, sigue los siguientes pasos:

1. Clonar el repositorio
git clone https://github.com/usuario/proyecto_churn.git
cd proyecto_churn
2. Crear un entorno virtual
python -m venv venv
3. Activar el entorno virtual

Windows

venv\Scripts\activate

Linux o Mac

source venv/bin/activate
4. Instalar dependencias
pip install -r requirements.txt
▶️ Ejecución del proyecto

El análisis y modelado se encuentran en el notebook:

Telecom_X_2.ipynb

Este archivo puede abrirse utilizando:

Jupyter Notebook

Google Colab

Visual Studio Code con la extensión de Python y Jupyter.

🤖 Modelos de Machine Learning utilizados

Durante el desarrollo del proyecto se entrenaron distintos modelos de clasificación:

Regresión Logística

Modelo estadístico utilizado para estimar la probabilidad de que un cliente cancele el servicio.

Árbol de Decisión

Modelo basado en reglas que divide los datos según las variables más relevantes para la clasificación.

Random Forest

Modelo de ensamble que combina múltiples árboles de decisión para mejorar la capacidad predictiva y reducir el sobreajuste.

📊 Evaluación de los modelos

Para evaluar el rendimiento de los modelos se utilizaron varias métricas de clasificación:

Accuracy

Precision

Recall

F1-score

Matriz de confusión

Estas métricas permiten analizar el desempeño de cada modelo y determinar cuál ofrece mejores resultados para la predicción de cancelación de clientes.

🔎 Principales factores que influyen en la cancelación

A partir del análisis realizado y de la importancia de variables en los modelos, se identificaron algunos factores que influyen significativamente en la cancelación de clientes, entre ellos:

Tipo de contrato del cliente

Antigüedad del cliente en la empresa

Cargos mensuales del servicio

Servicios adicionales contratados

Método de pago utilizado

Estos factores permiten entender mejor el comportamiento de los clientes y detectar posibles riesgos de cancelación.

💡 Conclusión

El uso de modelos de Machine Learning permitió identificar patrones relevantes asociados a la cancelación de clientes.

Los resultados obtenidos muestran que ciertas variables relacionadas con el tipo de contrato, la antigüedad del cliente y los cargos mensuales tienen un impacto importante en la probabilidad de cancelación.

A partir de estos hallazgos, las empresas pueden implementar estrategias orientadas a mejorar la retención de clientes, como incentivos para contratos de mayor duración, promociones personalizadas o programas de fidelización.

Este tipo de análisis permite tomar decisiones basadas en datos y anticiparse a posibles pérdidas de clientes.

👨‍💻 Autor

Eduin Rodríguez

Proyecto académico enfocado en el uso de técnicas de Machine Learning para la predicción de cancelación de clientes.
