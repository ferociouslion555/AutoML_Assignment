# Part 4 — RAPIDS cuML (GPU-accelerated ML)

GPU-accelerated machine learning with [RAPIDS cuML](https://docs.rapids.ai/api/cuml/stable/),
demonstrating dramatic speedups over CPU scikit-learn on the same algorithms.

## Notebook
- `rapids_cuml_automl.ipynb`

## What it covers
- Installing RAPIDS (cuDF + cuML) in Colab
- **GPU K-Means** with cuML and a CPU-vs-GPU timing comparison
- GPU classification/regression (e.g., Random Forest, Logistic/Linear Regression) with cuML
- Dimensionality reduction on GPU (PCA / UMAP)
- Benchmarking cuML vs scikit-learn on identical data

## Runtime
- **GPU is REQUIRED.** In Colab: `Runtime → Change runtime type → T4 GPU`.
- RAPIDS requires an NVIDIA GPU; it will not run on a CPU-only runtime.

## Install (first cell, Colab)
```python
# Colab ships with a RAPIDS-compatible CUDA; use the official installer
!pip install -q cudf-cu12 cuml-cu12 --extra-index-url=https://pypi.nvidia.com
```
> If the above fails on your Colab image, use the RAPIDS Colab install script:
> https://github.com/rapidsai/rapidsai-csp-utils

## How to run
1. Open `rapids_cuml_automl.ipynb` in Google Colab **with a GPU runtime**.
2. `Runtime → Run all`.
3. Save and commit the notebook **with outputs**.
