# 🧬 DisNetML: Disease Gene Prediction using Protein Interaction Networks

This project applies classical machine learning and deep learning techniques to predict disease-associated genes based on biological network features extracted from a human protein–protein interaction (PPI) network.

## Data Sources

- **[DG-AssocMiner](https://www.disgenet.org/downloads)** — disease–gene associations used for labeling (positive/negative).
- **[BioGRID (MITAB)](https://downloads.thebiogrid.org)** — comprehensive human PPI network for graph-based feature extraction.

## Features Extracted

From the PPI network, we extract multiple **graph topology features** for each gene:

- `Degree`
- `Betweenness Centrality`
- `Closeness Centrality`
- `Clustering Coefficient`
- `PageRank`
- `K-core number`
- `Shortest path to known disease genes`

## Models Used

- Classical: Random Forest, SVM, k-NN, Decision Tree, Naive Bayes
- Neural Models: MLP (ANN), DNN (Keras-based deep network)

## Objective

To build a machine learning pipeline that can distinguish between disease-causing and non-disease genes based on network context.

## Output

Model performance is evaluated using:

- **Accuracy**
- **AUROC**
- **Training Time**

Results are visualized in bar plots for comparison.

## File Structure

| File | Description |
|------|-------------|
| `disease_gene_pipeline.ipynb` | Main pipeline notebook |
| `README.md` | This file |
| `data/` | (optional) Local path to input files |

---

