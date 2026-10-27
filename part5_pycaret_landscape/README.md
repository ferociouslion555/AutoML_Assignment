# Part 5: PyCaret, capabilities landscape

A tour of PyCaret 3.3.2 across six kinds of problem, with synthetic datasets so every cell runs on the free CPU runtime.

## Notebook
`Copy_of_final_pycaret_capabilities_tour_(1).ipynb` (95 code cells, committed with outputs)

## Video walkthrough
https://www.youtube.com/watch?v=u8X83t8jL5g

## Video walkthrough
- https://www.youtube.com/watch?v=u8X83t8jL5g

## What it covers
- The three-line pattern: `setup`, `compare_models`, `predict_model`
- Binary classification (telecom churn), multiclass (loan grades) and regression (house prices)
- Tuning, bagging, blending, stacking and calibration
- Rare events: card fraud with SMOTE and cost-based thresholds
- Clustering (customer segments) and anomaly detection (transaction outliers)
- Time series with an exogenous promo input
- Text inside tables (product reviews)
- Interpretability: SHAP, reason codes and a fairness check
- Deployment: finalize, save, API file, and PSI drift monitoring
- **My run** (cell [95]): PyCaret classification on the breast cancer dataset

## Runtime
CPU only. **Runtime version 2025.07 (Python 3.11) is required.** In Colab: **Runtime > Change runtime type > Runtime version > 2025.07 > Save**. PyCaret 3.3.2 supports Python 3.9 to 3.11 only.

## Install (first cell)
```python
!pip install -q --only-binary=:all: "pycaret[analysis,models]==3.3.2"
```
After the install, use **Runtime > Restart session** and run the first cell again. A red "dependency resolver" error block is expected and harmless.

## Notes
- MLflow is not installed in my run; the notebook says so where it matters.
- Change from the reference Colab: the `pretty` table helper now handles string columns (pandas 3).
