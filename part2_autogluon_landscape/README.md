# Part 2 — AutoGluon: Landscape of Capabilities

A breadth tour of [AutoGluon](https://auto.gluon.ai/), AWS's open-source AutoML toolkit.

## Notebook
- `autogluon_landscape.ipynb`

## What it covers
- `TabularPredictor` for classification (Adult Income) and regression (California Housing)
- The model zoo + `leaderboard()`
- Predictions, probabilities, and permutation feature importance
- Overview of `MultiModalPredictor` (text/image) and `TimeSeriesPredictor` (forecasting)
- Presets (`best_quality` … `medium_quality`) and `time_limit` trade-offs

## Runtime
CPU works; GPU helps multimodal.

## Install (first cell)
```python
!pip install -q autogluon.tabular[all]
```

## How to run
1. Open in Colab, run the install cell, restart runtime if prompted.
2. `Runtime → Run all`.
3. Commit the notebook **with outputs**.
