# Robustness Evaluation: Repeatability, Reproducibility & Replicability

> **Author / Credits:** Created by [**@celine-am**](https://github.com/celine-am)

This repository contains the experimental summary data and visualization notebook ([`BoxPlots_Robustness.ipynb`](./BoxPlots_Robustness.ipynb)) evaluating the robustness of online anomaly detection models (**MOBKNN**, **subsetOBKNN**, and **OBKNN**) across **RMX** and **RMX-R** scenarios.

---

## Evaluation Scenarios

1. **Repeatability Test (`RMX`)** — *Team A (New) vs. Team A (Baseline)*  
   Evaluates consistency when repeating the same experiment under identical conditions by the same team.
2. **Reproducibility Test (`RMX`)** — *Team B (New) vs. Team A (Baseline)*  
   Evaluates consistency when the experiment is independently reproduced by a different team (**Team B**).
3. **Replicability Test (`RMX-R` vs. `RMX`)** — *Team A & Team B*  
   Evaluates model performance across scenarios (`RMX-R (New)` vs. `RMX (Baseline)`) for both teams.

---

## Repository Structure

```text
├── Baseline (Team A)/
│   ├── summary_results_baseline_RMX_MOBKNN.csv
│   ├── summary_results_baseline_RMX_subsetobknn.csv
│   ├── summary_results_baseline_RMX_OBKNN.csv
│   ├── summary_results_baseline_RMXR_MOBKNN.csv
│   ├── summary_results_baseline_RMXR_subsetobknn.csv
│   └── summary_results_baseline_RMXR_OBKNN.csv
├── Repeatability (Team A)/
│   ├── summary_results_repetabiliy_RMX_MOBKNN.csv
│   ├── summary_results_repetabiliy_RMX_subsetobknn.csv
│   └── summary_results_repetabiliy_RMX_OBKNN.csv
├── Robustness (Team B)/
│   ├── summary_results_RMX_MOBKNN.csv
│   ├── summary_results_RMX_subsetOBKNN.csv
│   ├── summary_results_RMX_OBKNN.csv
│   ├── summary_results_RMXR_MOBKNN.csv
│   ├── summary_results_RMXR_subsetOBKNN.csv
│   └── summary_results_RMXR_OBKNN.csv
├── BoxPlots_Robustness.ipynb
└── README.md
```

---

## Usage

Open [`BoxPlots_Robustness.ipynb`](./BoxPlots_Robustness.ipynb) in Jupyter Notebook, JupyterLab, or VS Code and run all cells to generate:
- Annotated AUC-PR boxplots (`Mean ± Std`) for each evaluation test.
- Publication-ready HTML and LaTeX (`booktabs`) summary tables.

---

## Attribution

Work and experimental results by [**Céline (@celine-am)**](https://github.com/celine-am).
