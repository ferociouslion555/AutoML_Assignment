# AutoML Assignment — Clustering & AutoML

This repository contains Google Colab notebooks (with full executed output) demonstrating
**K-Means clustering and its variations** along with three popular **AutoML** frameworks:
**PyCaret**, **AutoGluon**, and **RAPIDS cuML** (GPU-accelerated).

Each notebook was run end-to-end in Google Colab and committed **with its cell outputs preserved**
so the results are visible directly on GitHub without re-running anything.

---

## Repository structure

| Folder | Topic | Notebook | Runtime |
|--------|-------|----------|---------|
| [`part1_kmeans/`](./part1_kmeans) | K-Means and its variations | `kmeans_zero_to_hero.ipynb` | CPU |
| [`part2_pycaret/`](./part2_pycaret) | PyCaret AutoML (classification, regression, clustering) | `pycaret_automl.ipynb` | CPU |
| [`part3_autogluon/`](./part3_autogluon) | AutoGluon AutoML (tabular) | `autogluon_automl.ipynb` | CPU/GPU |
| [`part4_rapids_cuml/`](./part4_rapids_cuml) | RAPIDS cuML GPU-accelerated ML | `rapids_cuml_automl.ipynb` | **GPU required** |

---

## How to run

1. Open any `.ipynb` in Google Colab (click the file, then "Open in Colab", or upload it).
2. For **part4 (RAPIDS)**, set the runtime to **GPU**: `Runtime → Change runtime type → T4 GPU`.
3. `Runtime → Run all`.
4. `File → Save` and download the executed `.ipynb` (outputs are embedded) before committing.

Each part folder has its own `README.md` describing the notebook contents and key takeaways.

---

## Video walkthrough

A recorded walkthrough explaining each notebook cell-by-cell is linked here:

> **Video:** _(add your YouTube / unlisted video link here)_

---

## Deliverables checklist

- [ ] part1 — K-Means notebook runs top to bottom, committed with outputs
- [ ] part2 — PyCaret notebook runs top to bottom, committed with outputs
- [ ] part3 — AutoGluon notebook runs top to bottom, committed with outputs
- [ ] part4 — RAPIDS cuML notebook runs on GPU, committed with outputs
- [ ] Video walkthrough recorded and linked above
