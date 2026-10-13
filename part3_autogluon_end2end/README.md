# Part 3 — AutoGluon: End-to-End ML with Metrics

A deep, single-dataset AutoGluon workflow focused on evaluation and diagnostics
(Titanic survival, binary classification).

## Notebook
- `autogluon_end2end.ipynb`

## What it covers
- Data exploration + train/test split
- `TabularPredictor.fit()` with `best_quality` (bagging + stack ensembling)
- Leaderboard + `fit_summary()`
- Full metrics: accuracy, precision, recall, F1, ROC-AUC, log-loss
- Diagnostic plots: confusion matrix, ROC curve, precision-recall curve
- Permutation feature importance
- Save / load the predictor for deployment

## Runtime
CPU is fine.

## Install (first cell)
```python
!pip install -q autogluon.tabular[all] scikit-learn matplotlib seaborn
```

## How to run
1. Open in Colab, run the install cell, restart runtime if prompted.
2. `Runtime → Run all`.
3. Commit the notebook **with outputs**.
