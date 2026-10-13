# AutoML Assignment — Clustering & AutoML Frameworks

Google Colab notebooks (committed **with full executed output**) covering **K-Means clustering
and its variations** plus three major **AutoML** ecosystems: **AutoGluon**, **NVIDIA RAPIDS**,
and **PyCaret**.

Each notebook is designed to run top-to-bottom in Google Colab (`Runtime → Run all`) and is
committed with its cell outputs preserved, so results are visible on GitHub without re-running.

---

## Repository structure

| Part | Folder | Topic | Notebook | Runtime |
|------|--------|-------|----------|---------|
| 1 | [`part1_kmeans/`](./part1_kmeans) | K-Means and its variations | `Copy_of_final_kmeans_zero_to_hero.ipynb` | CPU |
| 2 | [`part2_autogluon_landscape/`](./part2_autogluon_landscape) | AutoGluon — landscape of capabilities | `autogluon_landscape.ipynb` | CPU |
| 3 | [`part3_autogluon_end2end/`](./part3_autogluon_end2end) | AutoGluon — end-to-end ML with metrics | `autogluon_end2end.ipynb` | CPU |
| 4 | [`part4_rapids_vs_cpu/`](./part4_rapids_vs_cpu) | NVIDIA RAPIDS vs CPU comparison | `rapids_vs_cpu.ipynb` | **GPU** |
| 5 | [`part5_pycaret_landscape/`](./part5_pycaret_landscape) | PyCaret — capabilities landscape | `pycaret_landscape.ipynb` | CPU |
| 6 | [`part6_pycaret_mlops/`](./part6_pycaret_mlops) | PyCaret — MLOps | `pycaret_mlops.ipynb` | CPU |

Each folder has its own `README.md` with the notebook contents, install cell, and run steps.

---

## How to run (any notebook)

1. Open the `.ipynb` in Google Colab (upload it, or use "Open in Colab").
2. **Part 4 (RAPIDS) only:** set a GPU runtime — `Runtime → Change runtime type → T4 GPU`.
3. Run the first cell (installs dependencies). Restart the runtime if Colab prompts, then continue.
4. `Runtime → Run all`.
5. `File → Download .ipynb` (outputs are embedded) and commit into the matching folder.

---

## Topics at a glance

- **Part 1 – K-Means:** from-scratch Lloyd's algorithm, k-means++, MiniBatch, Bisecting,
  choosing *k* (elbow + silhouette), failure cases vs GMM/Spectral/DBSCAN, image color quantization.
- **Part 2 – AutoGluon landscape:** `TabularPredictor` for classification + regression, model
  zoo leaderboard, feature importance, overview of multimodal & time-series predictors.
- **Part 3 – AutoGluon end-to-end:** one dataset in depth with a full metrics report
  (accuracy/precision/recall/F1/ROC-AUC/log-loss) and confusion/ROC/PR plots, save & load.
- **Part 4 – RAPIDS vs CPU:** cuDF/cuML vs pandas/scikit-learn benchmarks with speedup charts.
- **Part 5 – PyCaret landscape:** low-code AutoML across classification, regression, clustering,
  and anomaly detection.
- **Part 6 – PyCaret MLOps:** MLflow experiment tracking, model packaging, batch inference,
  and FastAPI/Docker deployment scaffolding.

---

## Video walkthrough

A recorded walkthrough explaining each notebook cell-by-cell:

> **Video:** _(add your YouTube / unlisted video link here)_

Each part can be its own video segment — see each folder's README for the talking points.

---

## Deliverables checklist

- [ ] Part 1 — K-Means notebook runs top to bottom, committed with outputs
- [ ] Part 2 — AutoGluon landscape notebook runs, committed with outputs
- [ ] Part 3 — AutoGluon end-to-end notebook runs, committed with outputs
- [ ] Part 4 — RAPIDS notebook runs on GPU, committed with outputs
- [ ] Part 5 — PyCaret landscape notebook runs, committed with outputs
- [ ] Part 6 — PyCaret MLOps notebook runs, committed with outputs
- [ ] Video walkthrough recorded and linked above
