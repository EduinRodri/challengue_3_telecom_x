# 📊 Telecom X: Predicción de Churn de Clientes

Este proyecto tiene como objetivo desarrollar un modelo de **Machine Learning** capaz de prever qué clientes tienen mayor probabilidad de cancelar sus servicios (*Churn*). Al anticiparse a este problema, la empresa puede implementar estrategias de retención proactivas y optimizar sus ingresos.

## 📂 Estructura del Proyecto

- `TelecomX_Churn_Prediction.ipynb`: Cuaderno principal con el pipeline completo (EDA, Preprocesamiento, Modelado).
- `telecomx_churn_limpio.csv`: Conjunto de datos tratado y listo para el modelado.
- `visualizaciones/`: (Opcional) Carpeta que contiene los gráficos de correlación, importancia de variables y matrices de confusión generados.

## ⚙️ Preparación de los Datos

El proceso de preparación fue riguroso para garantizar la calidad de las predicciones:

1.  **Clasificación de Variables**:
    - **Numéricas**: `tenure`, `MonthlyCharges`, `TotalCharges`.
    - **Categóricas**: `Contract`, `PaymentMethod`, `InternetService`, entre otras.
2.  **Codificación y Normalización**:
    - Se aplicó **One-Hot Encoding** a las variables categóricas.
    - Se utilizó **StandardScaler** para normalizar las variables numéricas en modelos sensibles a la escala (como Regresión Logística).
3.  **Tratamiento de Nulos**: Imputación por la mediana en la columna `TotalCharges`.
4.  **Balanceo de Clases**: Dado el desbalanceo original (~26% Churn), se utilizó la técnica **SMOTE** para equilibrar las clases al 50/50, permitiendo que el modelo aprenda patrones de cancelación de forma efectiva.
5.  **División de Datos**: Separación en 80% entrenamiento y 20% prueba utilizando partición estratificada.

## 🧠 Modelado y Justificación

Se entrenaron tres modelos de clasificación:
- **Regresión Logística**: Como modelo base de alta interpretabilidad.
- **Árbol de Decisión**: Para capturar reglas lógicas de negocio.
- **Random Forest (Modelo Elegido)**: Se seleccionó como modelo final debido a su robustez y superioridad en la métrica **Recall (84.3%)**, fundamental para no omitir clientes en riesgo.

## 📈 Insights y Visualización (EDA)

- **Contratos**: Los clientes con contratos "Mes a mes" son significativamente más propensos al Churn.
- **Antigüedad**: Existe una correlación negativa fuerte; a menor tiempo en la empresa, mayor riesgo de cancelación.
- **Método de Pago**: El uso de "Electronic Check" está vinculado a una mayor tasa de abandono.

## 🚀 Instrucciones de Ejecución

1.  Clona este repositorio.
2.  Asegúrate de tener instaladas las siguientes bibliotecas:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
    ```
3.  Carga el archivo `telecomx_churn_limpio.csv` en la misma carpeta que el cuaderno.
4.  Ejecuta todas las celdas del archivo `.ipynb` para replicar el análisis y los resultados.
