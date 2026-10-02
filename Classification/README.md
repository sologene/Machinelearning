# 🏷️ Classification

Predict a **category** (e.g. will a user buy a product: yes/no) from input features.

| Notebook | Algorithm | Key idea |
|----------|-----------|----------|
| [k_nearest_neighbors.ipynb](k_nearest_neighbors.ipynb) | K-Nearest Neighbors | Classifies by majority vote of the *k* closest points |
| [support_vector_machine.ipynb](support_vector_machine.ipynb) | SVM (linear) | Finds the widest-margin hyperplane between classes |
| [kernel_svm.ipynb](kernel_svm.ipynb) | Kernel SVM | Uses the kernel trick (RBF) for non-linear boundaries |
| [naive_bayes.ipynb](naive_bayes.ipynb) | Gaussian Naive Bayes | Applies Bayes' theorem assuming independent features |
| [decision_tree_classification.ipynb](decision_tree_classification.ipynb) | Decision Tree | Learns a tree of if/else rules |
| [random_forest_classification.ipynb](random_forest_classification.ipynb) | Random Forest | Ensemble of decision trees voting together |
| [Cancer B_M classification using catboost.ipynb](Cancer%20B_M%20classification%20using%20catboost.ipynb) | CatBoost | Gradient boosting to classify tumours as **Benign** or **Malignant** |

Every notebook evaluates the model with a **confusion matrix** and **accuracy score**.

## 📊 Dataset: `Social_Network_Ads.csv`

400 social network users and whether they bought a product after seeing an ad.

| Column | Description |
|--------|-------------|
| `Age` | User's age |
| `EstimatedSalary` | User's estimated salary |
| `Purchased` | `1` = bought, `0` = did not (target) |

## ▶️ Running the templates

Most notebooks here are **reusable templates** that load a generic `Data.csv`. To run them:

1. Copy `Social_Network_Ads.csv` (or any CSV with the target in the last column) to `Data.csv`, **or**
2. Change the `pd.read_csv(...)` line to point to your file.

The CatBoost notebook expects a breast-cancer dataset named `data.csv` (e.g. the [Wisconsin Breast Cancer dataset](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)).
