# Replication files

**Estimating Pair-Specific Network Effects in Binary-Action Games: Two-Sided Markets via Restricted Boltzmann Machines**  
Tetsuya Hoshino and Romans Pancs  
Accepted at *Management Science*.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tetsuyahoshino137/tetsuyahoshino137.github.io/blob/main/replication/hoshino-pancs/HoshinoPancs26MS.ipynb)

[Notebook](HoshinoPancs26MS.ipynb) · [Data and code (ZIP)](MS-BST-2025-01899.R2_replication.zip) · [Detailed README (PDF)](README.pdf) · [Author website](https://www.tetsuyahoshino.com/)

The notebook retains the original code and explanations of the model, equations, and algorithms.

## Run the simulation in Colab

1. Open the notebook and select **Runtime > Change runtime type > T4 GPU**. Estimation has been run in Google Colab; a GPU is required for practical computation.
2. Choose the settings in `Config` below. Use a fresh runtime for each figure.
3. Set `use_latex = False` in the optional **LaTeX Setting** cell to use Matplotlib fonts without installing LaTeX, then run the cells in order.

| Setting | Figure 3 (default) | Figure 4 |
| --- | --- | --- |
| `n1`, `n2` | `11`, `11` | `15`, `15` |
| `data_size` | `100_000` | `500_000` |
| `training_methods` | `['maximum_likelihood', 'contrastive_divergence']` | `['contrastive_divergence']` |

Keep the other settings unchanged. Each method takes about two hours, so Figure 3 takes about four hours and Figure 4 about two hours, plus data generation. The notebook generates its data; the ZIP is not needed for a new simulation.

## Plot the saved results

No new estimation or GPU is needed. Download and extract the ZIP, then:

1. In a fresh Colab session, run only the imports, device setup, and `Config` cells.
2. Use Colab's Files panel to upload the `training_data_*.json` files from **one** folder: `replication_package/results/figure3/` or `replication_package/results/figure4/`.
3. Set `use_latex = False`, run that cell, and run the final **Plotting Training Data** cell. Skip the data-generation and training cells. Set `download=True` in the final call if you want a PDF.

## Files and contact

The ZIP contains the code, synthetic observations, true parameters, full saved estimation histories, and detailed README. The separate [README.pdf](README.pdf) is identical to the PDF in the ZIP and also describes the package's command-line scripts.

Please cite the paper named above when using these materials.
