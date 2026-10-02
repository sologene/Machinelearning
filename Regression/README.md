# 📈 Regression

Predict a **continuous value** (e.g. salary) from one or more input features.

| Notebook | Algorithm | Key idea | Dataset |
|----------|-----------|----------|---------|
| [simple_linear_regression.ipynb](simple_linear_regression.ipynb) | Simple Linear Regression | Fits a straight line `y = b0 + b1·x` | `Salary_Data.csv`* |
| [multiple_linear_regression.ipynb](multiple_linear_regression.ipynb) | Multiple Linear Regression | Linear model with many features; one-hot encodes categorical columns | `50_Startups.csv`* |
| [polynomial_regression.ipynb](polynomial_regression.ipynb) | Polynomial Regression | Adds polynomial terms to capture non-linear trends | `Position_Salaries.csv` |
| [support_vector_regression.ipynb](support_vector_regression.ipynb) | SVR | Kernel-based regression (RBF); requires feature scaling | `Position_Salaries.csv` |
| [decision_tree_regression.ipynb](decision_tree_regression.ipynb) | Decision Tree Regression | Splits feature space into regions; better suited to multi-feature data | `Position_Salaries.csv` |
| [random_forest_regression.ipynb](random_forest_regression.ipynb) | Random Forest Regression | Averages many decision trees for a more stable prediction | `Position_Salaries.csv` |
| [logistic_regression.ipynb](logistic_regression.ipynb) | Logistic Regression | Despite the name, a **classifier**: predicts class probabilities | `Data.csv`* |

\* Not included in this folder. Add your own CSV with that name (features first, target last) to run the notebook.

## 📊 Dataset: `Position_Salaries.csv`

10 job positions with their level (1–10) and salary. Used to predict the salary for an intermediate level such as **6.5**.

| Column | Description |
|--------|-------------|
| `Position` | Job title |
| `Level` | Seniority level (feature) |
| `Salary` | Annual salary (target) |

## 🧠 Choosing a model

- **Linear relationship?** Start with Simple or Multiple Linear Regression.
- **Curved relationship, one feature?** Try Polynomial Regression or SVR.
- **Many features, non-linear?** Random Forest usually performs well out of the box.
