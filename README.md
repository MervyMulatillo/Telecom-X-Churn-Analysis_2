# Telecom-X-Churn-Analysis_2
# TelecomX-Predictive-Churn-Modeling
### Repositorio para el modelado predictivo y análisis de evasión (Churn) de Telecom X

---

## 📉 Modelado Predictivo de Evasión de Clientes (Churn) - Challenge Data Science

Este proyecto representa la fase avanzada del desafío de Data Science. Tras comprender el comportamiento histórico de los clientes de **Telecom X**, hemos desarrollado modelos de **Machine Learning** capaces de predecir qué clientes tienen mayor probabilidad de abandonar la empresa, permitiendo acciones preventivas y estratégicas basadas en datos.

### 🎯 Objetivo del Proyecto (Fase de Inteligencia Artificial)
Implementar un flujo completo de Ciencia de Datos Predictiva que incluya:
*   **Preprocesamiento Avanzado:** Limpieza de "Data Leakage" para evitar métricas ficticias, codificación de variables categóricas y normalización.
*   **Balanceo de Datos:** Aplicación de la técnica **SMOTE** para equilibrar las clases y mejorar drásticamente la detección de clientes en fuga.
*   **Modelado Multimodal:** Comparativa técnica entre modelos de optimización (**Regresión Logística**) y modelos basados en árboles (**Random Forest**).
*   **Evaluación de Alto Nivel:** Uso de métricas de industria como **AUC-ROC** y **Coeficiente de Gini** para medir la capacidad real de discriminación del modelo.
*   **Análisis de Importancia:** Identificar qué variables "pesan" más en la decisión de salida del cliente para priorizar estrategias de marketing.

### 🛠️ Tecnologías Utilizadas
*   **Python 3.12**
*   **Pandas & Numpy:** Preparación de matrices de datos y limpieza de nulos.
*   **Scikit-Learn:** Entrenamiento de modelos, escalado de datos y métricas de evaluación.
*   **Imbalanced-Learn (SMOTE):** Balanceo de clases desequilibradas para evitar sesgos.
*   **Matplotlib & Seaborn:** Generación de matrices de confusión, curvas ROC y análisis de importancia.

### 📈 Métricas y Visualizaciones Incluidas
1.  **Matriz de Confusión:** Visualización de aciertos, falsos positivos y falsos negativos (vital para medir el costo del error).
2.  **Curva ROC (Receiver Operating Characteristic):** Medición de la capacidad de separación del modelo frente al azar.
3.  **Gráfico de Importancia de Variables:** Identificación de los factores con mayor impacto predictivo en el Churn.
4.  **Reporte de Clasificación:** Detalle técnico de Exactitud, Precisión y el crítico **Recall**.

---

### Gráficos de Rendimiento (Modelado)

#### 1. Evaluación de Modelos: Matrices de Confusión y Curvas ROC
*Comparativa visual para determinar la capacidad de los modelos para distinguir entre clientes leales y en riesgo.*
<img width="435" height="147" alt="image" src="https://github.com/user-attachments/assets/4a4ed3f7-314c-43fd-a1af-73120d611343" />


---
#### 2. Top 10 Factores que determinan el Churn
*Análisis de las variables que el modelo identificó como críticas para predecir la evasión (Contratos, Cargos, Tenure).*
<img width="425" height="140" alt="image" src="https://github.com/user-attachments/assets/dc37c08d-a78b-4221-8a55-81877b2008db" />


---

### 📊 Resultados Obtenidos (Métricas Reales)

| Métrica | Regresión Logística (Ganadora) | Random Forest |
| :--- | :--- | :--- |
| **Exactitud (Accuracy)** | **77.09%** | 77.47% |
| **Recall (Sensibilidad)** | **63.81%** | 58.47% |
| **AUC-ROC** | **0.8240** | 0.8152 |
| **Coeficiente de Gini** | **0.6479** | 0.6304 |

> **Análisis Crítico:** Se seleccionó la **Regresión Logística** como el modelo estratégico para Telecom X debido a su superioridad en el **Recall (63.8%)**. En este negocio, es preferible detectar a un cliente que podría irse (aunque sea un falso positivo) que dejar escapar a uno que realmente va a cancelar.

---

### 💡 Conclusiones e Insights Predictivos
1.  **Poder de Discriminación (AUC 0.82):** El modelo demuestra una robustez alta para clasificar clientes según su nivel de riesgo, muy por encima del azar.
2.  **El "Gini" del Negocio (0.64):** Indica una excelente capacidad para rankear clientes. Telecom X puede ahora priorizar sus esfuerzos de retención enfocándose en el segmento de mayor puntaje generado por el modelo.
3.  **Variables Críticas:** El modelo confirma que el **Tipo de Contrato (Month-to-month)** y los **Cargos Mensuales elevados** son los disparadores principales de la evasión.

## 🚀 Cómo ejecutar este proyecto

1.  **Clona este repositorio:**
    ```bash
    git clone https://github.com/tu-usuario/TelecomX-Predictive-Churn-Modeling.git
    ```
2.  **Abre el archivo `.ipynb`** en Google Colab o Jupyter Notebook.
3.  **Asegúrate de tener instaladas las librerías necesarias:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn requests
    ```
4.  **Ejecuta el flujo completo:** Desde la limpieza de datos hasta la generación de las métricas de Gini y AUC.

---
#### **Autor:** [Mervy Mulatillo Piñin]
#### **Curso/Challenge:** Alura Latam - Challenge Data Science - Telecom X (Fase Predictiva)](https://github.com/MervyMulatillo/Telecom-X-Churn-Analysis_2/blob/main/README.md)
