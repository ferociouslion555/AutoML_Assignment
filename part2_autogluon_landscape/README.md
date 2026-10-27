# Part 2: AutoGluon, landscape of capabilities

A tour of what AutoGluon can do across problem types, using small synthetic datasets so every cell runs quickly.

## Notebook
`Copy_of_final_autogluon_capabilities_tour.ipynb` (85 code cells, committed with outputs)

## Video walkthrough
https://www.youtube.com/watch?v=DSapcsaV0sY

## What it covers
- The three-line pattern: `TabularPredictor(...).fit(...).predict(...)`
- Binary classification (telecom churn), multiclass classification (loan grades) and regression (house prices)
- Quantile regression for delivery-time windows
- Rare events: card fraud with `average_precision` and a cost curve
- Time series: store demand with known covariates, and Chronos
- Text plus tabular data (product reviews) and image classification (defect photos)
- Embeddings and semantic search over support tickets
- Tabular foundation models (TabPFN, Mitra) inside AutoGluon
- Interpretability, deployment, and a map of which module to use when
- **My run** (cell [84]): my own AutoGluon experiment, shown at the end of the notebook

## Runtime
CPU works. A GPU is not required. The free runtime has limited memory, so the Mitra foundation-model cell falls back with a short message if memory runs out.

## Install (first cell)
```python
!pip install --upgrade pip setuptools wheel
!pip install autogluon
```
Restart the runtime if Colab asks, then run from the top. AutoGluon 1.6.3 was used.

## Notes
- The last cell of the tour deletes `/tmp`. The **My run** cell recreates it at the start, so it runs correctly after a full run.
- Changes from the reference Colab: the `pretty` table helper now handles string columns (pandas 3), and the Mitra memory-error handler reads an empty error message safely.
- AutoGluon fits with time limits are not fully deterministic, so numbers can differ slightly between runs.
