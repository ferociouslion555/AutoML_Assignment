# AutoML Assignment: K-Means, AutoGluon, RAPIDS and PyCaret

CMPE 255 (Data Mining), Assignment 2, SJSU. Author: Ameya Mathew.

Six Google Colab notebooks covering K-means clustering and three AutoML ecosystems: AutoGluon, NVIDIA RAPIDS and PyCaret. Every notebook is committed with the full output of my own run, so the results can be read on GitHub without re-running anything. Each notebook ends with a **My run** cell: a short experiment of my own on a dataset or workload the original notebook does not use.

---

## Parts at a glance

| Part | Folder | Topic | Notebook | Runtime | My run cell | Open in Colab |
|---|---|---|---|---|---|---|
| 1 | [`part1_kmeans/`](./part1_kmeans) | K-means and its variations | `Copy_of_final_kmeans_zero_to_hero.ipynb` | CPU | [79] | [open](https://colab.research.google.com/github/ferociouslion555/AutoML_Assignment/blob/main/part1_kmeans/Copy_of_final_kmeans_zero_to_hero.ipynb) |
| 2 | [`part2_autogluon_landscape/`](./part2_autogluon_landscape) | AutoGluon: landscape of capabilities | `Copy_of_final_autogluon_capabilities_tour.ipynb` | CPU | [84] | [open](https://colab.research.google.com/github/ferociouslion555/AutoML_Assignment/blob/main/part2_autogluon_landscape/Copy_of_final_autogluon_capabilities_tour.ipynb) |
| 3 | [`part3_autogluon_end2end/`](./part3_autogluon_end2end) | AutoGluon: end-to-end ML with metrics | `Copy_of_final_autogluon_zero_to_hero.ipynb` | CPU | [105] | [open](https://colab.research.google.com/github/ferociouslion555/AutoML_Assignment/blob/main/part3_autogluon_end2end/Copy_of_final_autogluon_zero_to_hero.ipynb) |
| 4 | [`part4_rapids_vs_cpu/`](./part4_rapids_vs_cpu) | NVIDIA RAPIDS vs CPU | `Copy_of_final_nvidia_rapids_zero_to_hero.ipynb` | **T4 GPU** | [119] | [open](https://colab.research.google.com/github/ferociouslion555/AutoML_Assignment/blob/main/part4_rapids_vs_cpu/Copy_of_final_nvidia_rapids_zero_to_hero.ipynb) |
| 5 | [`part5_pycaret_landscape/`](./part5_pycaret_landscape) | PyCaret: capabilities landscape | `Copy_of_final_pycaret_capabilities_tour_(1).ipynb` | CPU, **Python 3.11** | [95] | [open](https://colab.research.google.com/github/ferociouslion555/AutoML_Assignment/blob/main/part5_pycaret_landscape/Copy_of_final_pycaret_capabilities_tour_%281%29.ipynb) |
| 6 | [`part6_pycaret_mlops/`](./part6_pycaret_mlops) | PyCaret: zero to hero and MLOps | `Copy_of_final_pycaret_zero_to_hero.ipynb` | CPU, **Python 3.11** | [137] | [open](https://colab.research.google.com/github/ferociouslion555/AutoML_Assignment/blob/main/part6_pycaret_mlops/Copy_of_final_pycaret_zero_to_hero.ipynb) |

The numbers in square brackets are the Colab execution labels shown beside each cell in the saved notebooks. Each folder has its own `README.md` with the contents, install steps and known notes.

---

## Video walkthroughs

Each video is a walkthrough of my own run in Colab, covering the important cells of the notebook.

| Part | Topic | Video |
|---|---|---|
| 1 | K-means and its variations | https://youtu.be/uMhKzvPJGS8 |
| 2 | AutoGluon: landscape of capabilities | https://www.youtube.com/watch?v=DSapcsaV0sY |
| 3 | AutoGluon: end-to-end ML with metrics | https://www.youtube.com/watch?v=xsPnw2ZNem8 |
| 4 | NVIDIA RAPIDS vs CPU | https://www.youtube.com/watch?v=ENIlUGNrE3c |
| 5 | PyCaret: capabilities landscape | https://www.youtube.com/watch?v=u8X83t8jL5g |
| 6 | PyCaret: zero to hero and MLOps | https://www.youtube.com/watch?v=Q2WS8I6nMK0 |

---

## How to run a notebook

1. Open the notebook with the **open** link above, or upload the `.ipynb` file to Colab.
2. Set the runtime before running anything (**Runtime > Change runtime type**):
   - Parts 1 to 3: CPU, default runtime version.
   - Part 4: **T4 GPU**.
   - Parts 5 and 6: CPU, and **Runtime version 2025.07**. This is the Python 3.11 image. PyCaret 3.3.2 supports Python 3.9 to 3.11 only, and the first cell stops with a message if the version is wrong.
3. Run the first (install) cell. If Colab asks for it, use **Runtime > Restart session**, then run the install cell again.
4. Use **Runtime > Run all** and wait for the run to finish. Parts 5 and 6 take the longest.
5. To save a run: **File > Download > Download .ipynb** (outputs are embedded in the file), then commit it into the matching folder.

A red "dependency resolver" error block after `pip install` in Parts 5 and 6 is expected and harmless. The notebook explains why.

---

## Changes from the reference Colabs

The notebooks are partly cloned from the reference Colabs given in the assignment. I ran them in my own environment and made the minimum changes needed for them to run to the end:

| Part | Change |
|---|---|
| 2 | Replaced the `pretty` table helper (it failed on string columns with pandas 3); fixed the Mitra memory-error handler; the My run cell recreates the temp folder that the last tour cell deletes. |
| 4 | Replaced the `pretty` table helper for the same pandas 3 problem. |
| 5 | Replaced the `pretty` table helper for the same pandas 3 problem. |
| 6 | The `setup(use_gpu=True)` demo cell now checks that a GPU is attached and skips the flag on a CPU runtime. The original cell crashed the session. |

Each folder README lists these again with the exact cell.

---

## Deliverables checklist

- [x] Part 1: K-means notebook runs top to bottom, committed with outputs
- [x] Part 2: AutoGluon landscape notebook runs, committed with outputs
- [x] Part 3: AutoGluon end-to-end notebook runs, committed with outputs
- [x] Part 4: RAPIDS notebook runs on a T4 GPU, committed with outputs
- [x] Part 5: PyCaret landscape notebook runs, committed with outputs
- [x] Part 6: PyCaret MLOps notebook runs, committed with outputs
- [x] Video walkthroughs recorded and linked above (all 6 parts)
- [x] My run cell in every notebook
