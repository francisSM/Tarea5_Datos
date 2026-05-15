# Tarea5_Datos: Predicción de Riesgo de Salud Materna

Este repositorio contiene un experimento completo de Machine Learning enfocado en predecir el nivel de riesgo de salud durante el embarazo, utilizando indicadores fisiológicos clave.

## Visualizar el Experimento
Puedes explorar el análisis de datos, el código completo y las métricas de rendimiento abriendo directamente el siguiente Jupyter Notebook:

**[Maternal_Health_Risk_Experiment.ipynb](./Maternal_Health_Risk_Experiment.ipynb)**

*(Nota: GitHub renderiza automáticamente el Notebook para que puedas leerlo sin necesidad de descargar nada).*

## Contexto del Proyecto
El objetivo principal de este proyecto es construir un modelo predictivo capaz de clasificar el riesgo materno en tres niveles: `low risk`, `mid risk` y `high risk`. Esta clasificación busca servir como una herramienta de apoyo a la decisión clínica para identificar tempranamente casos críticos.

### Contenido del Notebook
El experimento sigue una estructura rigurosa:
1. **Análisis Exploratorio de Datos (EDA):** Resumen estadístico, mapa de correlaciones y análisis de la distribución de clases.
2. **Definición y Diseño Experimental:** Partición estratificada (80/20) y escalado de datos (`StandardScaler`).
3. **Modelado Comparativo:** Se entrenan y comparan dos arquitecturas:
   - **Random Forest**
   - **Support Vector Machine (SVM)**
4. **Análisis Clínico:** Una discusión orientada a la salud sobre por qué minimizar los **falsos negativos en casos de alto riesgo** es el factor más crítico, y cómo el Random Forest demuestra ser la opción más fiable para este entorno.

## Dataset
Los datos utilizados provienen del **UCI Machine Learning Repository**:
- **Dataset:** [Maternal Health Risk Dataset (ID: 863)](https://archive.ics.uci.edu/dataset/863/maternal+health+risk)
- Se descarga automáticamente dentro del Notebook usando la librería oficial `ucimlrepo`.