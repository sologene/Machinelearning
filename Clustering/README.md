# 🔵 Clustering

**Unsupervised learning**: group similar data points together without any labels.

| Notebook | Algorithm | Key idea |
|----------|-----------|----------|
| [k_means_clustering.ipynb](k_means_clustering.ipynb) | K-Means | Uses the **Elbow Method** to pick *k*, then groups customers into 5 clusters |
| [hierarchical_clustering.ipynb](hierarchical_clustering.ipynb) | Hierarchical (Agglomerative) | Builds a **dendrogram** to choose the number of clusters |
| [catboost.ipynb](catboost.ipynb) | CatBoost | Gradient boosting classifier (a copy of the one in [Classification](../Classification/)) |

## 📊 Dataset: `Mall_Customers.csv`

200 mall customers. The goal is to segment them by **annual income** and **spending score** so the mall can target marketing.

| Column | Description |
|--------|-------------|
| `CustomerID` | Unique ID |
| `Genre` | Gender |
| `Age` | Age |
| `Annual Income (k$)` | Yearly income in thousands of dollars |
| `Spending Score (1-100)` | Score assigned by the mall based on spending behaviour |

## 🎯 Result

Both methods reveal distinct customer segments, such as *high income / low spending* ("careful") and *high income / high spending* ("target") customers.
