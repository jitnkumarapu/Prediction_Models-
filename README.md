# Prediction Models

A curated collection of machine learning example projects. Each subfolder contains a Jupyter notebook, a dataset (CSV), and a short description. The notebooks demonstrate typical ML workflows: data loading, EDA, feature preparation, modeling, and evaluation.

Quick start
-----------
1. Create and activate a Python virtual environment:

```bash
python -m venv .venv
# Windows PowerShell
.\.venv\Scripts\Activate.ps1
# Windows CMD
.venv\\Scripts\\activate.bat
```

2. Install common dependencies (adjust per-notebook as needed):

```bash
pip install --upgrade pip
pip install pandas numpy scikit-learn matplotlib seaborn jupyterlab notebook
# Optional: tensorflow, keras, xgboost
pip install tensorflow keras xgboost
```

3. Open a notebook (example):

```bash
jupyter lab "Prediction models/Heart Stroke Prediction/Stroke detection.ipynb"
```

Repository structure
-------------------
See the `DESCRIPTION.md` file for a concise overview of the included projects and datasets.

Contributing
------------
- Add improvements to existing notebooks (cleaner preprocessing, stronger baselines).
- Add a per-project `requirements.txt` if a notebook needs non-standard libraries.
- Document dataset provenance or preprocessing steps in the project folder.

Licensing & Data
----------------
Datasets are stored in the respective project folders. Verify license and usage rights for each dataset before sharing or publishing results.

Contact
-------
If you want help extending these notebooks or packaging them into reproducible experiments, open an issue or ask for assistance.
