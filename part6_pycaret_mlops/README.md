# Part 6: PyCaret, zero to hero and MLOps

One synthetic budgeting dataset (1,500 households, predicting who will overspend next month) followed through PyCaret 3.3.2, from a first experiment to a saved pipeline, an API file and drift monitoring.

## Notebook
`Copy_of_final_pycaret_zero_to_hero.ipynb` (140 code cells, committed with outputs)

## Video walkthrough
https://www.youtube.com/watch?v=Q2WS8I6nMK0

## What it covers
- The lifecycle, a hand-built baseline, and a first PyCaret experiment
- The `setup` preprocessing knobs, one at a time (imputation, scaling, multicollinearity, outliers, SMOTE, polynomial features and more)
- Classification: compare, metrics and the plot gallery
- Tuning, ensembles, calibration and cost-based thresholds
- Regression and a deliberate leakage trap
- Interpretability: SHAP, reason codes, permutation importance and partial dependence
- Clustering, anomaly detection and time series (one series, and a panel model)
- MLOps: finalize, save and reload, predicting on new data, the generated API and Docker files, experiment logging, a fairness check, PSI drift and retraining
- Error analysis and a 12-point diagnostics checklist
- Where low-code ML fits in the 2026 landscape
- **My run** (cell [137]): finalize, save, reload, predict and a PSI drift check on the breast cancer dataset

## Runtime
CPU only. **Runtime version 2025.07 (Python 3.11) is required.** In Colab: **Runtime > Change runtime type > Runtime version > 2025.07 > Save**. PyCaret 3.3.2 supports Python 3.9 to 3.11 only. A full run takes a while, so keep the tab open.

## Install (first cell)
```python
!pip install -q --only-binary=:all: "pycaret[analysis,models]==3.3.2"
```
After the install, use **Runtime > Restart session** and run the first cell again. A red "dependency resolver" error block is expected and harmless.

## Notes
- Not installed in my run, and the notebook handles it: MLflow, `evidently` (so `check_drift` is shown but not run), cuML and the tabular foundation models (a stand-in estimator is used).
- Change from the reference Colab: the `setup(use_gpu=True)` demo cell now checks that a GPU is attached and skips the flag on a CPU runtime. The original cell crashed the session.
- One cell prints a long stream of LightGBM warnings. They are harmless.
