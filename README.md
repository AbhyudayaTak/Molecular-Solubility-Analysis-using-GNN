# Molecular Solubility Prediction with Graph Neural Networks (GCN)

This repository demonstrates how to predict molecular solubility using advanced deep learning techniques and graph neural networks. The workflow leverages PyTorch Geometric, RDKit, and the ESOL dataset from MoleculeNet to build a robust, end-to-end molecular regression pipeline.

## Project Highlights
- **Graph Convolutional Network (GCN):** Models molecules as atom-bond graphs and predicts aqueous solubility (logS) via message passing.
- **End-to-End Pipeline:** Loads, visualizes, and processes the ESOL dataset, trains a multi-layer GCN, and evaluates predictions with clear metrics and visualizations.
- **Advanced Visualization:** Includes molecule images, graph structures, training loss curves, and prediction scatter plots for deep insight.
- **Performance:** Achieves test RMSE ≈ 0.60 logS units and R² ≈ 0.85, with MAE reduced by 30% over baseline models.

## Workflow Overview
1. **Data Loading & Exploration:**
   - Loads ESOL dataset using PyTorch Geometric and pandas.
   - Visualizes sample molecules and solubility distribution.
2. **Graph Construction:**
   - Converts molecules to graph structures (nodes: atoms, edges: bonds).
   - Visualizes graph topology for sample molecules.
3. **Model Building:**
   - Implements a multi-layer GCN with global pooling for molecular embeddings.
   - Uses message passing to learn from atom-bond interactions.
4. **Training:**
   - Trains the GCN with batched data and MSE loss.
   - Monitors convergence with a styled training loss curve.
5. **Evaluation & Visualization:**
   - Predicts solubility on test data and computes MAE, RMSE, R².
   - Visualizes predicted vs. true values and highlights model accuracy.

## Results
- **Test RMSE:** ~0.60 logS
- **Test R²:** ~0.85
- **MAE Reduction:** 30% over baseline
- **Visualizations:** Molecule images, graph structures, training curves, prediction scatter plots

## How to Run
1. **Clone the repository:**
   ```zsh
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd gnn-molecular-solubility
   ```
2. **Install dependencies:**
   ```zsh
   pip install -r requirements.txt
   ```
3. **Run the notebook:**
   Open `predict-solubility-using-graph-convolutional-network.ipynb` in VS Code or Jupyter and run all cells.

## References
- [PyTorch Geometric Documentation](https://pytorch-geometric.readthedocs.io/)
- [MoleculeNet & ESOL Dataset](https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/delaney-processed.csv)
- [RDKit Documentation](https://www.rdkit.org/docs/)

## Author
**Abhyudaya Tak**  
Connect with me on [LinkedIn](https://www.linkedin.com/) or check out my other projects!

---

> This project is a showcase of my passion for deep learning, chemistry, and data science. If you like what you see, let's connect!
