# 🏦 Lending Club — Loan Default Prediction

Proyecto Integrador de Aprendizaje Automático — Clasificación supervisada con scikit-learn y PySpark + LIME.

## 📖 Ver el Jupyter Book

👉 **[https://Jumsc.github.io/Machine-Learning-Uninorte](https://Jumsc.github.io/Machine-Learning-Uninorte)**

## 📋 Descripción

Modelo de clasificación para predecir si un préstamo de Lending Club resultará en default, usando:

- **EDA completo** con PySpark sobre 1.3M registros
- **scikit-learn** RandomForest + GridSearchCV
- **PySpark** RandomForest + CrossValidator
- **LIME** para interpretabilidad local
- **Comparación** de métricas y tiempos entre frameworks

## 🗂️ Estructura

```
lending_club_book/
├── _config.yml          # Configuración del libro
├── _toc.yml             # Tabla de contenidos
├── intro.md             # Página de inicio
├── LendingClub.ipynb    # Notebook principal
└── requirements.txt     # Dependencias
```

## 🚀 Ejecutar localmente

```bash
pip install jupyter-book
jupyter-book build lending_club_book/
open lending_club_book/_build/html/index.html
```

## 📊 Resultados

| Métrica | scikit-learn | PySpark |
|---|---|---|
| ROC AUC | 0.7115 | 0.7118 |
| F1-score | 0.6987 | 0.6921 |
| Tiempo total | ~324s | ~2099s* |

*En Windows local. En Colab con Linux: significativamente más rápido.

## 🛠️ Tecnologías

Python · PySpark 3.5 · scikit-learn · LIME · Matplotlib · Seaborn
