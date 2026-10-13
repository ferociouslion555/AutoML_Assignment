# Part 2 — PyCaret AutoML

Low-code AutoML with [PyCaret](https://pycaret.org/): automated preprocessing, model
comparison, tuning, and interpretation across multiple task types.

## Notebook
- `pycaret_automl.ipynb`

## What it covers
- `setup()` — automated preprocessing pipeline (imputation, encoding, scaling)
- **Classification**: `compare_models()` to leaderboard many models, `tune_model()`, `plot_model()`
- **Regression**: end-to-end regression workflow
- **Clustering**: unsupervised module (`create_model('kmeans')`, `assign_model()`)
- Model interpretation (feature importance, SHAP where available)
- `finalize_model()` and `predict_model()` on holdout data

## Runtime
- CPU is sufficient.

## Install (first cell)
```python
!pip install -q pycaret
```

## How to run
1. Open `pycaret_automl.ipynb` in Google Colab.
2. `Runtime → Run all`.
3. Save and commit the notebook **with outputs**.
