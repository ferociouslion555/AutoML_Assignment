# Part 3 — AutoGluon AutoML

Automated machine learning with [AutoGluon](https://auto.gluon.ai/): train high-accuracy
tabular models with a single `fit()` call, including automatic ensembling and stacking.

## Notebook
- `autogluon_automl.ipynb`

## What it covers
- `TabularPredictor` for **classification** and **regression**
- Automatic feature preprocessing and multi-layer stack ensembling
- `predictor.leaderboard()` to compare the trained model zoo
- `fit_summary()`, feature importance, and evaluation on test data
- `presets` trade-offs (`best_quality` vs `medium_quality`) and `time_limit`

## Runtime
- CPU works; GPU speeds up some models.

## Install (first cell)
```python
!pip install -q autogluon.tabular
```

## How to run
1. Open `autogluon_automl.ipynb` in Google Colab.
2. `Runtime → Run all`.
3. Save and commit the notebook **with outputs**.
