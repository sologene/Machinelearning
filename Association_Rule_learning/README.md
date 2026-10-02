# 🛒 Association Rule Learning

Discover **"people who bought X also bought Y"** rules from transaction data.

| Notebook | Algorithm | Key idea |
|----------|-----------|----------|
| [apriori.ipynb](apriori.ipynb) | Apriori | Ranks rules by **support**, **confidence** and **lift** |
| [Eclat.ipynb](Eclat.ipynb) | Eclat | Simplified version that ranks item sets by **support** only |

## 📊 Dataset: `Market_Basket_Optimisation.csv`

7,501 transactions from a grocery store over one week. Each row is one customer's basket (up to 20 items).

## 📐 Key metrics

| Metric | Meaning |
|--------|---------|
| **Support** | How often an item set appears in all transactions |
| **Confidence** | How often Y is bought when X is bought |
| **Lift** | How much more likely Y is bought with X than on its own (> 1 means a real association) |

## 📦 Extra dependency

```bash
pip install apyori
```
