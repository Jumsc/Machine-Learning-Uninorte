# 🏦 Lending Club — Loan Default Prediction

**Proyecto Integrador de Aprendizaje Automático**

---

## Descripción

Este proyecto implementa un modelo de clasificación supervisada para predecir si un préstamo emitido por la plataforma **Lending Club** resultará en default (1) o será pagado completamente (0).

Se comparan dos entornos de procesamiento:

- **scikit-learn** — para modelado local con GridSearchCV
- **PySpark** — para procesamiento distribuido con CrossValidator

Además se aplica **LIME** para interpretar las predicciones del modelo.

---

## Dataset

| Característica | Detalle |
|---|---|
| Nombre | Lending Club Loan Data (2007–2020) |
| Fuente | Kaggle |
| Registros válidos | 1,345,310 |
| Columnas | 151 |
| Variable objetivo | `default` (0 = Fully Paid, 1 = Charged Off) |

---

## Estructura del proyecto

```{tableofcontents}
```

---

## Resultados principales

| Métrica | scikit-learn | PySpark |
|---|---|---|
| ROC AUC | 0.7115 | 0.7118 |
| F1-score | 0.6987 | 0.6921 |
| Tiempo total | ~324s | ~2099s (Windows) |

> **Nota:** Los tiempos reflejan ejecución en Windows local. En Google Colab con Linux y `parallelism=4`, PySpark es significativamente más rápido.

---

## Tecnologías utilizadas

- Python 3.x
- PySpark 3.5
- scikit-learn
- LIME
- Matplotlib / Seaborn
