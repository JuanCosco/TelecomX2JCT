# Telecom X – Parte 2

## Predicción de Cancelación de Clientes (Churn)

---

## 📌 Descripción del Proyecto

Este proyecto forma parte del desafío **Telecom X – Parte 2**, cuyo objetivo es desarrollar modelos de *Machine Learning* capaces de predecir la cancelación de clientes (*churn*).

A partir del análisis exploratorio realizado previamente, en esta etapa se construyó un pipeline de modelado para anticipar qué clientes tienen mayor probabilidad de abandonar el servicio, permitiendo a la empresa diseñar estrategias de retención basadas en datos.

---

## 🎯 Objetivos

* Preparar los datos para el modelado (tratamiento, codificación, normalización).
* Realizar análisis de correlación y selección de variables.
* Entrenar dos o más modelos de clasificación.
* Evaluar el rendimiento de los modelos con métricas.
* Interpretar los resultados, incluyendo la importancia de las variables.
* Crear una conclusión estratégica señalando los principales factores que influyen en la cancelación.

---

## Tecnologías Utilizadas

* Pandas
* NumPy
* Matplotlib / Seaborn
* Scikit-learn

---

## Pipeline del Proyecto

### 1) Preprocesamiento

* Eliminación de variables irrelevantes.
* Tratamiento de valores nulos.
* Codificación de variables categóricas (One-Hot Encoding).
* Normalización de variables numéricas cuando fue necesario.
* División en conjunto de entrenamiento y prueba.

### 2) Modelado

Se entrenaron dos modelos de clasificación:

* **Regresión Logística**
* **Random Forest**

### 3) Evaluación

Se utilizaron las siguientes métricas:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC
* Matriz de Confusión


## Principales Factores de Cancelación

Entre las variables más influyentes se identificaron:

* Tipo de contrato (mensual vs largo plazo)
* Antigüedad del cliente (tenure)
* Cargos mensuales elevados
* Servicios adicionales contratados
* Método de pago

---

## 💡 Estrategias de Retención Propuestas

* Incentivar contratos a largo plazo.
* Ofrecer beneficios progresivos según antigüedad.
* Revisar estructura de precios para clientes de alto riesgo.
* Implementar campañas preventivas basadas en scoring predictivo.
* Diseñar ofertas personalizadas según perfil de riesgo.

