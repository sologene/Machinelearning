<div align="center">

# 🤖 Machine Learning Toolkit

**A hands-on collection of machine learning algorithms, from regression to deep learning, implemented in Jupyter notebooks with real datasets.**

![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)

</div>

---

## 📖 About

This repository is a toolkit of **30+ machine learning notebooks**, grouped by learning paradigm. Each folder contains self-contained notebooks along with the dataset they use, so you can open any notebook and run it top to bottom.

Every notebook follows the same workflow:

1. **Import libraries**
2. **Load the dataset**
3. **Preprocess** (encoding, feature scaling, train/test split)
4. **Train** the model
5. **Predict and evaluate** (confusion matrix, accuracy, plots)
6. **Visualise** the results

---

## 🗂️ Repository Structure

| # | Module | What's inside | Dataset(s) |
|---|--------|---------------|------------|
| 0 | [**Data Preprocessing**](data_preprocessing_tools.ipynb) | Missing values, encoding, splitting, feature scaling | `Data.csv` |
| 1 | [**Regression**](Regression/) | Simple / Multiple / Polynomial Linear, SVR, Decision Tree, Random Forest, Logistic | `Position_Salaries.csv` |
| 2 | [**Classification**](Classification/) | KNN, SVM, Kernel SVM, Naive Bayes, Decision Tree, Random Forest, CatBoost | `Social_Network_Ads.csv` |
| 3 | [**Clustering**](Clustering/) | K-Means, Hierarchical | `Mall_Customers.csv` |
| 4 | [**Association Rule Learning**](Association_Rule_learning/) | Apriori, Eclat | `Market_Basket_Optimisation.csv` |
| 5 | [**Reinforcement Learning**](Reinforcement_learning/) | Upper Confidence Bound, Thompson Sampling | `Ads_CTR_Optimisation.csv` |
| 6 | [**Natural Language Processing**](Natural_Language_Processing/) | Bag-of-Words sentiment analysis | `Restaurant_Reviews.tsv` |
| 7 | [**Deep Learning**](Deep_Learning/) | Artificial Neural Network, Convolutional Neural Network | `Churn_Modelling.csv`, cats vs dogs images |
| 8 | [**Dimensionality Reduction**](Dimensionality_Reduction/) | PCA, LDA, Kernel PCA | `Wine.csv` |
| 9 | [**Model Selection & Boosting**](Model%20selection_and_boosting/) | k-Fold Cross Validation, XGBoost | `Social_Network_Ads.csv` |

Each folder has its own `README.md` with a description of every notebook.

```
Machinelearning/
├── data_preprocessing_tools.ipynb
├── Regression/
├── Classification/
├── Clustering/
├── Association_Rule_learning/
├── Reinforcement_learning/
├── Natural_Language_Processing/
├── Deep_Learning/
│   └── dataset for CNN/      # 10,000 cat & dog images
├── Dimensionality_Reduction/
├── Model selection_and_boosting/
└── requirements.txt
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/sologene/Machinelearning.git
cd Machinelearning
```

> ⚠️ The CNN image dataset is ~240 MB, so the clone may take a moment.

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter

```bash
jupyter notebook
```

Then open any notebook. Run it **from inside its folder** so the relative dataset path resolves.

> 💡 **Prefer the cloud?** Upload a notebook and its dataset to [Google Colab](https://colab.research.google.com/) and run it there, no install needed.

---

## 🧰 Tech Stack

| Purpose | Libraries |
|---------|-----------|
| Data handling | `numpy`, `pandas` |
| Visualisation | `matplotlib` |
| Classical ML | `scikit-learn`, `scipy` |
| Boosting | `xgboost`, `catboost` |
| Deep learning | `tensorflow` / `keras` |
| NLP | `nltk` |
| Association rules | `apyori` |

---

## 📝 Notes

- Some notebooks are general-purpose **templates** that read a placeholder file (e.g. `Data.csv`). Drop in any CSV where the last column is the target and they will run as-is.
- All datasets are small, public, educational datasets commonly used for learning ML.

---

## 🤝 Contributing

Found a bug or want to add an algorithm? Open an issue or a pull request, contributions are welcome.

<div align="center">

⭐ **If you find this useful, consider giving the repo a star!** ⭐

</div>
