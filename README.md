# Artificial-Intelligence-Assignments

**23F-6014 · Amama Sajjad · AI 2002 · Spring 2026 · NUCES FAST**

---

## File 1 — `23F-6014_AI_A4_Q2_Simulation.ipynb`
**Assignment 4, Q2: Minimax & Alpha-Beta Pruning (Tic-Tac-Toe)**

Fully automated Tic-Tac-Toe where MAX (X) and MIN (O) both play using Minimax + Alpha-Beta pruning. No human input — runs start to finish.

- Utility: +1 (X wins), -1 (O wins), 0 (draw)
- Set `verbose=True` in `simulate_game()` to print α/β values at every node
- Expected output: DRAW · Nodes visited: 21,652 · Cutoffs: 9,601

**Run:** `jupyter notebook 23F-6014_AI_A4_Q2_Simulation.ipynb`

---

## File 2 — `Q2_Clustering_Scratch.ipynb`
**Assignment 7, Q2: K-Means & K-Medoids from Scratch**

K-Means and K-Medoids built using only NumPy/pandas/matplotlib. No sklearn.

- Includes elbow plots, cluster visualisations, convergence trace, timing
- Requires `clustering_dataset.csv` in the same folder
- `np.random.seed(42)` set globally for reproducibility

**Run:** `jupyter notebook Q2_Clustering_Scratch.ipynb`

---

## File 3 — `Q3_Clustering_Sklearn.ipynb`
**Assignment 7, Q3: K-Means & K-Medoids via Scikit-Learn**

Same experiment as Q2 but using sklearn. K-Medoids uses a custom wrapper (`KMedoidsSK`) with `sklearn.metrics.pairwise_distances` because `scikit-learn-extra` breaks on NumPy 2.x.

- Direct SSE + timing comparison against scratch implementations
- `linear_sum_assignment` (scipy) used for cluster label alignment
- Requires `clustering_dataset.csv` in the same folder

**Run:** `pip install scikit-learn scipy` then `jupyter notebook Q3_Clustering_Sklearn.ipynb`

---

## File 4 — `f236014_AI_A3__1_.ipynb`
**Assignment 3, Section C: Local Search Algorithms**

Maximises f(x) = −(x−3)² + 9 (global max = 9 at x=3) using three algorithms:

- Simple Hill Climbing (first-choice)
- Steepest-Ascent Hill Climbing
- Simulated Annealing
- Local Beam Search

Each prints a step-by-step trace + matplotlib trajectory plot.

**Run:** `jupyter notebook f236014_AI_A3__1_.ipynb`

---

## File 5 — `AI_A4_23f-6014_Amama_Q2report.docx`
**Assignment 4, Q2: Written Report**

Formal report accompanying File 1. Covers: objective, game implementation, agent design, alpha-beta explanation, simulation walkthrough, results, and conclusion.

---

## Dependencies
```
pip install numpy pandas matplotlib scikit-learn scipy
```
