# Part 3: AutoGluon, end-to-end ML with metrics

One problem followed in depth: a synthetic budgeting dataset of 1,500 households, predicting who will overspend next month. The notebook covers metrics, thresholds, calibration, leakage, tuning, explanation, time series, deployment and drift.

## Notebook
`Copy_of_final_autogluon_zero_to_hero.ipynb` (107 code cells, committed with outputs)

## Video walkthrough
https://www.youtube.com/watch?v=xsPnw2ZNem8

## What it covers
- The AutoML promise and its limits; a first predictor in three lines
- Data analysis, the metric families for classification, and the leaderboard beyond the score
- Imbalance, decision thresholds chosen by cost, and calibration
- Regression and quantile regression, and a deliberate leakage trap
- Presets and time budgets, bagging and stacking, and hyperparameter search
- Permutation importance and per-prediction explanations
- Time series forecasting with `TimeSeriesPredictor` and Chronos
- Text notes plus numbers (category vs text vs transformer)
- MLOps: persist and reload, `refit_full`, `clone_for_deployment`, distillation, latency, PSI drift and monitoring
- Error analysis and a diagnostics checklist
- The 2026 tabular frontier: foundation models, TabArena and what to use when
- **My run** (cell [105]): AutoGluon regression on the California housing dataset (20,640 rows)

## Runtime
CPU is enough. The time limits in the notebook are short because it is designed for the free runtime.

## Install (first cell)
```python
!pip install --upgrade pip setuptools wheel
!pip install autogluon
```
Restart the runtime if Colab asks, then run from the top.

## Notes
- Fits are time-limited, so numbers can differ slightly between runs.
- Two optional model families fall back with a message on the free runtime: the multimodal fine-tune and TabICL. The notebook says so where it happens.
