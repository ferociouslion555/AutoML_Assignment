# Part 1: K-means and its variations

A "zero to hero" notebook on K-means clustering, from the algorithm itself to variants, validity metrics, real applications and deployment.

## Notebook
`Copy_of_final_kmeans_zero_to_hero.ipynb` (79 code cells, committed with outputs)

## Video walkthrough
https://youtu.be/uMhKzvPJGS8

## What it covers
- Foundations: what a cluster is, the prototype, the objective, and why the centroid is the mean
- Lloyd's algorithm from scratch, convergence, and scikit-learn `KMeans`
- Initialisation: the random-start trap, k-means++, empty clusters and outliers
- Bisecting K-means, from scratch and in scikit-learn
- Variants: K-medians, spherical K-means, K-medoids (PAM), Mini-Batch K-means, fuzzy c-means, Gaussian mixtures (EM) and kernel K-means
- Validity: internal and external metrics, the similarity matrix, a statistical test for structure, and choosing K with elbow, silhouette, gap statistic and stability
- Failure cases (sizes, densities, shapes) and K-means vs hierarchical vs DBSCAN
- Applications: customer segmentation, colour quantisation and digits
- Explainability, error analysis, a pipeline with persistence, and monitoring drift
- Embeddings (text, images, multimodal), deep clustering and the 2026 toolbox
- **My run** (cell [79]): my own K-means experiment, shown at the end of the notebook

## Runtime
CPU is enough. The libraries used are preinstalled in Colab; the install line at the top is commented out.

## How to run
1. Open the notebook in Colab.
2. Use **Runtime > Run all**.
3. To save a run: **File > Download > Download .ipynb**, then commit it into this folder.
