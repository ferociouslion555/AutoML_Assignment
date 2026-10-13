# Part 6 — PyCaret: MLOps

The MLOps lifecycle around a PyCaret model: experiment tracking, packaging,
and deployment scaffolding.

## Notebook
- `pycaret_mlops.ipynb`

## What it covers
- `setup(log_experiment=True)` → automatic **MLflow** experiment logging
- Training with tracked runs; querying runs via `mlflow.search_runs`
- `save_model` / `load_model` — portable pipeline artifacts
- Batch inference with `predict_model`
- `create_api` / `create_docker` — FastAPI + Docker productionization scaffolding

## Runtime
CPU is sufficient.

## Install (first cell)
```python
!pip install -q pycaret mlflow
```

## How to run
1. Open in Colab, run the install cell, restart runtime if prompted.
2. `Runtime → Run all`.
3. Commit the notebook **with outputs**.
