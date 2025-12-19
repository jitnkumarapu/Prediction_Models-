# Prediction Models — Applied Machine Learning Portfolio

A concise, interview‑ready portfolio of end‑to‑end supervised learning projects demonstrating reproducible workflows, defensible validation, and clear actionable results. Each project is self-contained with a primary notebook, datasets (or pointers), model artifacts, and a short report.

Badges: <!-- add CI / PyPI / license badges here -->

## Table of contents
- Key highlights
- Technologies
- How to run locally
- Repository structure
- Project index (select projects)
- Scripts & utilities
- Reproducibility & best practices
- Contributing
- Contact & license

## Key highlights
- Focus: practical supervised learning (classification & regression) with interpretability and robust validation.
- Artifacts: Jupyter notebooks, saved models, evaluation metrics, and visual diagnostics (ROC/PR, residuals, feature importance, SHAP).

## Technologies
- Python, JupyterLab, pandas, NumPy, scikit-learn, XGBoost, LightGBM, SHAP, matplotlib, seaborn
- Competencies: data cleaning, feature engineering, cross-validation (stratified & time-aware), hyperparameter tuning, interpretability, reproducibility

## How to run locally
1. Clone and open the repository:
   git clone <repo-url>
   cd "Prediction_Models"
2. Create and activate a virtual environment:
   python -m venv .venv
   # Windows PowerShell:
   .\.venv\Scripts\Activate.ps1
3. Install dependencies:
   pip install -r requirements.txt
4. Launch JupyterLab:
   jupyter lab

## Repository structure
See DESCRIPTION.md for a concise overview of included projects and datasets.
Typical top-level layout:
- DESCRIPTION.md — short repo overview and dataset notes
- <project-name>/* — project folder with primary notebook (*.ipynb), data/ (or pointers), models/, and README
- scripts/ — auxiliary utilities (indexing, evaluation)
- requirements.txt — base environment
- LICENSE, CODE_OF_CONDUCT.md (optional)

## Project index (select projects)
- **Breast Cancer Prediction**
  - Description: Predicts diagnosis (M = malignant, B = benign) from clinical features.
  - Technologies: Logistic Regression, Decision Tree
  - Results: Logistic Regression — 97% accuracy; Decision Tree — 93.5% accuracy
  - Artifacts: notebook, model pickles, confusion matrix, feature importance

- **Heart Stroke Prediction**
  - Description: Predicts stroke risk using demographics and medical features.
  - Technologies: Logistic Regression, SVM, Decision Tree, KNN
  - Results: Logistic Regression / SVM / KNN — ~93.8% accuracy

- **House Price Prediction**
  - Description: Predicts house prices using location, area, bedroom/bathroom counts, and engineered features.
  - Technologies: Linear Regression, Ridge, Random Forest Regressor
  - Results: Random Forest Regressor — 87.89%

- **Medical Cost Prediction**
  - Description: Predicts treatment costs from age, gender, BMI, smoking status, etc.
  - Technologies: Linear & Polynomial Regression, Decision Tree, Random Forest
  - Results: Decision Tree & Random Forest performed well

- **Room Occupancy Detection**
  - Description: Predicts room occupancy using sensor telemetry (temperature, light, CO2).
  - Technologies: Random Forest Classifier
  - Results: Random Forest — 98% accuracy

- **Sleep Disorder Prediction**
  - Description: Predicts sleep disorders from lifestyle and medical features.
  - Technologies: Random Forest, Decision Tree
  - Results: Random Forest — 89% accuracy

- **Pima Indians Diabetes Prediction**
  - Description: Predict diabetes presence among female patients using clinical indicators.
  - Technologies: Logistic Regression, Random Forest, SVM
  - Results: Logistic Regression — 78% accuracy

- **Salary Prediction**
  - Description: Predicts salaries from demographics, experience, job title, country, and other features.
  - Technologies: Decision Tree Regressor, Random Forest Regressor
  - Results: Random Forest — 94.6%

- **Loan Approval Prediction**
  - Description: Predicts whether a bank will approve a loan application.
  - Technologies: Decision Tree, Random Forest
  - Results: Decision Tree — 91.4% accuracy

- **Warranty Claims Fraud Prediction**
  - Description: Predicts authenticity of warranty claims across region, category, and claim value.
  - Technologies: Decision Tree, Random Forest, Logistic Regression
  - Results: Models in the 91–92% range

- **E‑Commerce Product Delivery Prediction**
  - Description: Predicts on‑time delivery for international e‑commerce shipments.
  - Technologies: Decision Tree, Random Forest, Logistic Regression, KNN
  - Results: Decision Tree — 69% accuracy

- **Hotel Reservation Cancellation Prediction**
  - Description: Predicts reservation cancellations using booking and customer features.
  - Technologies: Decision Tree, Random Forest, Logistic Regression
  - Results: Decision Tree — 85% accuracy

- **Indian Used Car Price Prediction**
  - Description: Predicts used car prices for Indian metro cities using vehicle and market features.
  - Technologies: Decision Tree, Random Forest
  - Results: Random Forest — 87.8% accuracy

## Scripts & utilities
- scripts/generate_project_index.py — (suggested) enumerate projects and primary notebooks
- scripts/run_notebook_ci.sh — (optional) headless notebook execution for CI
- Per-project: consider adding requirements.txt when using non-standard packages

## Reproducibility & best practices
- Validation: stratified k-folds, time-aware splits where appropriate, held-out test sets.
- Interpretability: SHAP summaries, calibration plots, subgroup performance analyses.
- Artifacts: notebooks include random seeds, environment notes, and saved model artifacts.

## Contributing
Guidelines for contributors:
- Improve notebooks: cleaner preprocessing, stronger baselines, documented experiments.
- Per-project requirements: add a requirements.txt inside the project folder for non-standard deps.
- Document provenance: add dataset source, license, and preprocessing steps in project README or data/README.md.
- Tests & CI: add lightweight checks (e.g., execute notebook cells) before merging.
- PR workflow:
  - Fork → feature branch → open PR with clear description and artifacts
  - Include reproducibility notes and short changelog in PR
  - Prefer small, focused PRs for notebooks (one logical change per PR)
- Issues: open an issue before major changes or dataset additions.

## Contact & license
- Author: (Your Name) — Data Scientist. Add email and GitHub profile here.
- License: Add LICENSE file (e.g., MIT) and reference here.

Quick tasks I can add on request:
- Create scripts/generate_project_index.py
- Add CI notebook execution (GitHub Actions)
- Generate per-project README template and requirements.txt

<!-- end of file -->
