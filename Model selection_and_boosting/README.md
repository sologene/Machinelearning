# 🏆 Model Selection & Boosting

Evaluate models more reliably and boost their performance.

| Notebook | Technique | Key idea |
|----------|-----------|----------|
| [k_fold_cross_validation.ipynb](k_fold_cross_validation.ipynb) | k-Fold Cross Validation | Trains and tests on 10 different splits to get a robust accuracy estimate (mean ± std) for a Kernel SVM |
| [xg_boost.ipynb](xg_boost.ipynb) | XGBoost | Fast, high-performing gradient-boosted trees, evaluated with a confusion matrix and k-fold CV |

## 📊 Dataset: `Social_Network_Ads.csv`

400 users with `Age`, `EstimatedSalary` and whether they `Purchased` a product after seeing an ad.

The XGBoost notebook is a **template** that reads `Data.csv`. Point it at `Social_Network_Ads.csv` or your own CSV (target in the last column).

## 📦 Extra dependency

```bash
pip install xgboost
```
