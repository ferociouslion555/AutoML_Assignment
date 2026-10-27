# Part 5 — PyCaret: Capabilities Landscape

A breadth tour of [PyCaret](https://pycaret.org/), the low-code AutoML library,
across every task type.

## Notebook
- `pycaret_landscape.ipynb`

## Video walkthrough
- https://www.youtube.com/watch?v=u8X83t8jL5g

## What it covers
- `setup()` automated preprocessing pipeline
- **Classification**: `compare_models`, `tune_model`, `plot_model` (AUC/confusion/feature)
- **Regression**: end-to-end with residual/error plots
- **Clustering**: `create_model('kmeans')`, `assign_model`, cluster + elbow plots
- **Anomaly detection**: Isolation Forest
- `finalize_model` / `predict_model` / `save_model`

## Runtime
CPU is sufficient.

## Install (first cell)
```python
!pip install -q pycaret
```

## How to run
1. Open in Colab, run the install cell, restart runtime if prompted.
2. `Runtime → Run all`.
3. Commit the notebook **with outputs**.
