# Transparent-Credit-Risk-Scoring-with-Explainable-AI

💳 Transparent Credit Risk Scoring with Explainable AI
Predict credit default risk with **accuracy**, **fairness**, and **transparency** — all while aligning with modern financial regulations like **FCRA** and **GDPR**.
This project integrates **machine learning**, **explainable AI**, and **regulatory reporting** to build a fully transparent credit scoring pipeline that could be used by FinTech companies, banks, or regulators.

## 📌 Project Overview
In real-world financial systems, **model predictions aren't enough**. Institutions must **justify** their decisions to regulators and consumers. This project addresses that need by:
- Predicting loan default risk using machine learning.
- Providing human-readable explanations with SHAP/LIME.
- Generating auditable reports and mock regulatory notices.
- Optionally detecting demographic bias in model behavior.

## ⚙️ Tech Stack
| Category             | Tools Used                                                                  |
|----------------------|-----------------------------------------------------------------------------|
| Data Processing      | `pandas`, `numpy`, `scikit-learn`, `imbalanced-learn`, `pandas-profiling`   |
| Modeling             | `XGBoost`, `LightGBM`, `optuna`, `scikit-learn`                             |
| Explainability       | `SHAP`, `LIME`, `Eli5`                                                      |
| Fairness & Bias      | `Fairlearn`, `AIF360`                                             |
| Reporting            | `Jinja2`, `WeasyPrint`, `logging`, `datetime`, `uuid`                       |
| Visualization        | `matplotlib`, `seaborn`, `plotly`, `streamlit`                              |
| API & Deployment     | `FastAPI`, `Docker`, `GitHub Actions`                            |

## 🛠️ Features
### ✅ Credit Default Prediction
- Trained model (XGBoost/LightGBM) on public datasets (e.g., LendingClub/UCI Credit).
- Metrics: AUC, F1-score, Precision/Recall, Confusion Matrix.

### ✅ Explainability Layer
- Global Feature Importance (SHAP summary plots).
- Local Prediction Explanations (SHAP force plots, LIME).
- Counterfactual suggestions (optional): *"If you increased income by $X..."*

### ✅ Regulatory Reporting Simulation
- Human-readable explanation generator for loan rejections.
- Exports PDF rejection notices using
