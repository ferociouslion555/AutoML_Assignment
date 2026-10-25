# Part 1 — K-Means and its Variations

A "zero to hero" tour of K-Means clustering and its common variants.

## Notebook
- `Copy_of_final_kmeans_zero_to_hero.ipynb`

## Video walkthrough
- https://youtu.be/uMhKzvPJGS8

## What it covers
- K-Means intuition and Lloyd's algorithm (implemented from scratch with NumPy)
- scikit-learn `KMeans` on synthetic data
- Choosing **k**: the elbow method (inertia) and silhouette analysis
- **K-Means++** vs random initialization
- **MiniBatchKMeans** for large datasets (speed vs quality)
- **Bisecting K-Means** (hierarchical divisive variant)
- Where K-Means fails + alternatives (GaussianMixture, Spectral, DBSCAN)
- Application: **image color quantization**
- Metrics: inertia, silhouette, Davies–Bouldin, adjusted Rand index

## Runtime
CPU is sufficient.

## How to run
1. Open the notebook in Google Colab.
2. `Runtime → Run all`.
3. Save and commit the notebook **with outputs**.
