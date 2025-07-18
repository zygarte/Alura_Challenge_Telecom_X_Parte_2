# Alura_Challenge_Telecom_X_Parte_2


# 🤖 Telecom X - Predicción de Cancelación de Clientes (Churn)

Este proyecto forma parte de la segunda etapa del análisis de clientes de Telecom X. Luego de explorar y comprender los datos, el objetivo ahora es construir modelos de Machine Learning que predigan qué clientes tienen mayor probabilidad de cancelar sus servicios.

---

## 🎯 Objetivos

- Preparar y transformar los datos tratados previamente.
- Entrenar y comparar al menos dos modelos de clasificación.
- Evaluar el rendimiento con métricas relevantes.
- Identificar variables clave que influyen en la cancelación.
- Proponer recomendaciones estratégicas basadas en los resultados.

---

## ⚙️ Flujo del Proyecto

### 1. Preprocesamiento

- Carga de los datos tratados desde JSON.
- Eliminación de columnas irrelevantes como `customerID`.
- Conversión del target `Churn` a variable binaria (`Churn_bin`).
- Aplicación de one-hot encoding para variables categóricas.
- División del dataset en entrenamiento y prueba.
- Normalización de variables para modelos sensibles a escala.

### 2. Modelado

Se entrenaron y evaluaron dos modelos:

- **Regresión Logística:** Modelo lineal que requiere datos normalizados.
- **Random Forest:** Ensamble de árboles de decisión, robusto frente a datos no escalados.

Ambos modelos se evaluaron usando:

- Matriz de confusión
- Exactitud (Accuracy)
- Precisión
- Recall
- F1-score

---

## 🔍 Principales Hallazgos

- El modelo **Random Forest** obtuvo mejor rendimiento global.
- Las variables más influyentes fueron: tipo de contrato, método de pago, servicios contratados y gasto mensual.
- Los clientes con contratos mensuales y pagos electrónicos son más propensos a cancelar.

---

## 💡 Recomendaciones

- **Incentivar contratos de largo plazo** (anuales o trimestrales).
- Identificar clientes con alto gasto y contrato mensual para aplicar retención anticipada.
- Ofrecer promociones personalizadas a clientes con mayor riesgo de churn.
- Integrar este modelo a sistemas de atención al cliente para acciones proactivas.

---

## 📁 Archivos Incluidos

- `TelecomX_Prediccion_Cancelacion.ipynb` – Notebook con todo el pipeline de Machine Learning.
- `TelecomX_Data.json` – Fuente de datos tratada desde la Parte 1.
- `README.md` – Descripción del proyecto y metodología utilizada.

---

## 🚀 Próximos Pasos

- Validar modelos con más datos históricos.
- Explorar técnicas de balanceo (SMOTE, undersampling).
- Integrar modelos en tiempo real para monitoreo de churn.

