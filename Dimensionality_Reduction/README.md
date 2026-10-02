# 📉 Dimensionality Reduction

Compress many features into a few while keeping the important information, then train a classifier on the reduced data.

| Notebook | Technique | Type | Key idea |
|----------|-----------|------|----------|
| [principal_component_analysis.ipynb](principal_component_analysis.ipynb) | PCA | Unsupervised | Finds directions of **maximum variance** |
| [linear_discriminant_analysis.ipynb](linear_discriminant_analysis.ipynb) | LDA | Supervised | Finds directions that best **separate the classes** |
| [kernel_pca.ipynb](kernel_pca.ipynb) | Kernel PCA | Unsupervised | PCA with a kernel (RBF) for **non-linear** data |

Each notebook reduces the 13 features to **2 components**, trains a **Logistic Regression** model, and plots the decision regions.

## 📊 Dataset: `Wine.csv`

178 wines described by 13 chemical properties (alcohol, malic acid, flavanoids, colour intensity, proline, ...). The target `Customer_Segment` (1, 2 or 3) groups wines by the kind of customer who likes them.
