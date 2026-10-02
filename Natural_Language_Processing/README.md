# 💬 Natural Language Processing

Sentiment analysis: predict whether a **restaurant review is positive or negative**.

| Notebook | Technique |
|----------|-----------|
| [natural_language_processing.ipynb](natural_language_processing.ipynb) | Bag-of-Words model + Random Forest classifier |

## 🔄 Pipeline

1. **Clean the text**: remove punctuation and numbers, lowercase everything
2. **Remove stopwords** (keeping "not", since it flips sentiment)
3. **Stem** words with the Porter Stemmer (`loved` → `love`)
4. **Bag of Words**: `CountVectorizer` turns each review into a word-count vector
5. **Train a Random Forest classifier** (100 trees) and evaluate it with a confusion matrix

## 📊 Dataset: `Restaurant_Reviews.tsv`

1,000 restaurant reviews, tab-separated.

| Column | Description |
|--------|-------------|
| `Review` | Review text |
| `Liked` | `1` = positive, `0` = negative (target) |

## 📦 Extra setup

```bash
pip install nltk
python -c "import nltk; nltk.download('stopwords')"
```
