# Part 4 — NVIDIA RAPIDS vs CPU

Benchmark GPU-accelerated [RAPIDS](https://rapids.ai/) (cuDF + cuML) against CPU
pandas / scikit-learn on identical tasks.

## Notebook
- `rapids_vs_cpu.ipynb`

## Video walkthrough
- https://www.youtube.com/watch?v=ENIlUGNrE3c

## What it covers
- DataFrame groupby: **cuDF** vs pandas
- **K-Means**: cuML vs scikit-learn
- **Random Forest**: cuML vs scikit-learn
- **Logistic Regression**: cuML vs scikit-learn
- **PCA**: cuML vs scikit-learn
- A speedup summary table + bar charts

## Runtime
**GPU REQUIRED.** In Colab: `Runtime → Change runtime type → T4 GPU`.
RAPIDS will not run on a CPU-only runtime.

## Install (first cell, Colab)
```python
!pip install -q cudf-cu12 cuml-cu12 --extra-index-url=https://pypi.nvidia.com
```
> If this fails on your Colab image, use the RAPIDS Colab installer:
> https://github.com/rapidsai/rapidsai-csp-utils

## How to run
1. Set a **GPU** runtime, run the install cell, restart if prompted.
2. `Runtime → Run all`.
3. Commit the notebook **with outputs**.
