# 📡 TelecomX – Parte 2: Predicción de Churn con Machine Learning

Segunda etapa del proyecto TelecomX. A partir del análisis exploratorio previo(https://github.com/JuanCosco/TelecomXJCT)), se construyó un pipeline de Machine Learning para predecir la cancelación de clientes (*churn*), comparando dos modelos de clasificación y formulando estrategias de retención basadas en los resultados.

---

## 🎯 Objetivo

Desarrollar modelos predictivos que identifiquen clientes con alta probabilidad de cancelar el servicio, permitiendo a la empresa diseñar intervenciones de retención basadas en datos.

---

## 🔄 Pipeline

```
telecomx_clean.csv (output Parte 1)
        ↓
   Preprocesamiento
   (encoding, normalización, train/test split)
        ↓
   Entrenamiento de modelos
   (Logistic Regression / Random Forest)
        ↓
   Evaluación de métricas
        ↓
   Interpretación de variables
        ↓
   Conclusiones estratégicas
```

---

## 📊 Resultados de los modelos

| Métrica | Logistic Regression | Random Forest |
|---------|-------------------|---------------|
| Accuracy | 0.74 | **0.76** |
| Precision | 0.51 | **0.53** |
| Recall | 0.78 | **0.79** |
| F1-Score | 0.61 | **0.63** |
| ROC AUC | 0.840 | **0.846** |

El **Random Forest ajustado** obtiene el mejor desempeño general. Ambos modelos convergen en los mismos factores clave de churn, lo que refuerza la confiabilidad de los resultados.

---

## 🔍 Principales factores de cancelación

**Incrementan el churn:**
- Servicio de internet por fibra óptica (Odds Ratio ≈ 1.52)
- Pago por electronic check
- Facturación electrónica
- Servicios de streaming y líneas múltiples

**Reducen el churn:**
- Antigüedad del cliente *(principal predictor en ambos modelos)*
- Contratos a 2 años → reducción significativa
- Contratos a 1 año → reducción moderada
- Soporte técnico contratado
- Seguridad online

---

## 💡 Estrategias de retención propuestas

- **Onboarding estructurado** para clientes nuevos — la antigüedad es el factor dominante
- **Incentivos a contratos largos** — anuales y bianuales
- **Monitoreo preventivo** del segmento fibra óptica
- **Beneficios por migración** a métodos de pago recurrentes (débito automático)
- **Inclusión de soporte técnico y seguridad** en paquetes base

---

## 🛠️ Stack tecnológico

| Herramienta | Uso |
|-------------|-----|
| Python 3 | Lenguaje principal |
| Pandas / NumPy | Preprocesamiento y transformación |
| Scikit-learn | Modelado y evaluación |
| Matplotlib / Seaborn | Visualizaciones |
| Jupyter Notebook | Desarrollo y documentación |

---

## 📁 Estructura del repositorio

```
TelecomX2JCT/
├── DataScience.ipynb       # Notebook con pipeline completo de ML
├── telecomx_clean.csv      # Dataset limpio (output de Parte 1)
└── README.md
```

---

## 🚀 Cómo ejecutar

```bash
git clone https://github.com/JuanCosco/TelecomX2JCT.git
cd TelecomX2JCT

pip install pandas numpy matplotlib seaborn scikit-learn jupyter

jupyter notebook DataScience.ipynb
```

---

## 🔗 Serie del proyecto

| Parte | Descripción | Repo |
|-------|-------------|------|
| Parte 1 | ETL + EDA | [TelecomXJCT](https://github.com/JuanCosco/TelecomXJCT) |
| Parte 2 | ML Predictivo | ← estás aquí |

---

## 👤 Autor

**Juan Armando Cosco Turín**  
[GitHub](https://github.com/JuanCosco)
