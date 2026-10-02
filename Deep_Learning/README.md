# 🧠 Deep Learning

Neural networks built with **TensorFlow / Keras**.

| Notebook | Model | Task | Dataset |
|----------|-------|------|---------|
| [artificial_neural_network.ipynb](artificial_neural_network.ipynb) | Artificial Neural Network (ANN) | Predict whether a bank customer will **leave the bank** | `Churn_Modelling.csv` |
| [convolutional_neural_network.ipynb](convolutional_neural_network.ipynb) | Convolutional Neural Network (CNN) | Classify an image as a **cat or a dog** | `dataset for CNN/` |

---

## 🏦 ANN: Customer Churn

**Dataset:** 10,000 bank customers with features such as credit score, geography, gender, age, tenure, balance and activity status. The target `Exited` is `1` if the customer left.

**Architecture:**
- Input → Dense(6, ReLU) → Dense(6, ReLU) → Dense(1, Sigmoid)
- Optimizer: Adam · Loss: binary cross-entropy · 100 epochs

---

## 🐱🐶 CNN: Cats vs Dogs

**Dataset:** 10,000 images

| Split | Cats | Dogs |
|-------|------|------|
| Training | 4,000 | 4,000 |
| Test | 1,000 | 1,000 |

**Architecture:**
- Image augmentation with `ImageDataGenerator` (rescale, shear, zoom, flip)
- Conv2D → MaxPool → Conv2D → MaxPool → Flatten → Dense(128) → Dense(1, Sigmoid)
- 64×64 input images · 25 epochs

> ⚠️ **Path note:** the notebook reads images from `dataset/training_set` and `dataset/test_set`. Either rename `dataset for CNN/` to `dataset/`, or update the paths in the notebook. For the single-image prediction cell, add an image at `dataset/single_prediction/cat_or_dog_1.jpg`.

> 💡 Training a CNN on CPU is slow. A GPU runtime on [Google Colab](https://colab.research.google.com/) speeds it up a lot.
