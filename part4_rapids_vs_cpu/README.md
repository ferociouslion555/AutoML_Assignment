# Part 4: NVIDIA RAPIDS vs CPU

RAPIDS (cuDF, cuML and friends) compared with pandas and scikit-learn on the same tasks, measured on a free Colab T4 GPU. The notebook also shows where the CPU still wins.

## Notebook
`Copy_of_final_nvidia_rapids_zero_to_hero.ipynb` (120 code cells, committed with outputs)

## Video walkthrough
https://www.youtube.com/watch?v=ENIlUGNrE3c

## What it covers
- Why GPUs help, the T4, and a first benchmark that counts the copy cost
- cuDF as pandas on the GPU, and `cudf.pandas` (zero code change)
- Data analysis and plotting from GPU frames, and the small-data trap
- cuML classification (the scikit-learn API), all metric families, thresholds and calibration
- cuML regression and preprocessing pipelines that stay on the GPU
- Clustering (k-means, DBSCAN, HDBSCAN), PCA, UMAP, t-SNE, nearest neighbours and anomaly scores
- Cross-validation and grid search, and `cuml.accel`
- Scaling up: memory, dtype shrinking, the RMM pool, spilling, chunked Parquet and Dask-cuDF
- XGBoost and SHAP on the GPU; a spending graph (cuGraph is not installed in my run, so it ran on NetworkX)
- Saving, serving latency and drift; error analysis and diagnostics
- Where CPUs still win: small data, single-row serving and Python UDFs
- **My run** (cell [119]): random forest, k-means and groupby timed on CPU and GPU at 50,000, 200,000 and 500,000 rows

## Runtime
**T4 GPU required.** In Colab: **Runtime > Change runtime type > T4 GPU**. RAPIDS does not run on a CPU-only runtime. The notebook was run with RAPIDS 26.06.

## Install
RAPIDS 26.06 was available on the T4 runtime I used. If `import cudf` fails on a fresh runtime, uncomment this line at the top of Part 0 and restart the session:
```python
!pip install -q cudf-cu12 cuml-cu12 cugraph-cu12 --extra-index-url=https://pypi.nvidia.com
```

## Notes
- GPU timings vary a little between runs.
- Change from the reference Colab: the `pretty` table helper now handles string columns (pandas 3).
