# Part 1 — K-Means and its Variations

A "zero to hero" tour of K-Means clustering and its common variants.

## Notebook
- `kmeans_zero_to_hero.ipynb`

## What it covers
- K-Means intuition and the Lloyd's algorithm (implemented from scratch with NumPy)
- scikit-learn `KMeans` on synthetic and real datasets
- Choosing **k**: the elbow method (inertia) and silhouette analysis
- **K-Means++** vs random initialization
- **MiniBatchKMeans** for large datasets (speed vs quality trade-off)
- **Bisecting K-Means** (hierarchical divisive variant)
- Comparison with other clustering methods (e.g., Gaussian Mixture / Spectral)
- A practical application: **image color quantization**
- Evaluation metrics: inertia, silhouette score, Davies–Bouldin, adjusted Rand index

## Runtime
- CPU is sufficient.

## How to run
1. Open `kmeans_zero_to_hero.ipynb` in Google Colab.
2. `Runtime → Run all`.
3. Save and commit the notebook **with outputs**.
