# Machine Learning From Scratch

A growing collection of classic machine learning algorithms implemented **from scratch** using only Python and NumPy to understand the internal mechanics of each algorithm. Built to understand exactly how each algorithm works under the hood: the math, the optimization process, and the logic behind every prediction.

**13 machine learning algorithms implemented from scratch using Python and NumPy.**

![Python](https://img.shields.io/badge/Python-100%25-blue?logo=python)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Stars](https://img.shields.io/github/stars/fares-ahmed7/Machine-Learning-From-Scratch?style=social)
![Last Commit](https://img.shields.io/github/last-commit/fares-ahmed7/Machine-Learning-From-Scratch)

---

## 📑 Table of Contents

- [Overview](#-overview)
- [Implemented Algorithms](#-implemented-algorithms)
- [Project Structure](#-project-structure)
- [Installation](#️-installation)
- [Usage](#-usage)
- [Roadmap](#-roadmap)
- [Project Goals](#-project-goals)
- [Tech Stack](#️-tech-stack)
- [Contributing](#-contributing)
- [References](#-references)
- [License](#-license)
- [Author](#-author)

---

## 📖 Overview

Most machine learning libraries abstract away the implementation details behind a single `.fit()` call. This repository does the opposite: every algorithm is implemented step by step using plain Python and NumPy, making it easier to understand exactly what happens during training and prediction — from gradient descent and distance calculations to decision boundaries and splitting criteria.

This repository is designed as a learning resource for anyone who wants to:

- Understand the mathematical foundations of machine learning algorithms
- Learn how popular algorithms work internally without relying on black-box libraries
- Explore clean, minimal, and well-documented implementations
- Compare their own implementations with a reference implementation
- Build a solid foundation before using libraries such as scikit-learn or PyTorch

---

## 🧠 Implemented Algorithms

| Algorithm | File | Category | Core Idea |
|---|---|---|---|
| Linear Regression | `linear_regression.py` | Regression | Fits a line by minimizing MSE via gradient descent |
| Logistic Regression | `logistic_regression.py` | Classification | Applies the sigmoid function to model class probabilities |
| Perceptron | `perceptron.py` | Classification | Learns a linear decision boundary via iterative weight updates |
| K-Nearest Neighbors (KNN) | `K-Nearest_Neighbors.py` | Classification | Predicts the majority label among the *k* closest points |
| Decision Tree | `decision_tree.py` | Classification / Regression | Recursively splits data using information gain / variance reduction |
| Random Forest | `random_forest.py` | Ensemble Learning | Aggregates predictions from many bagged decision trees |
| AdaBoost | `adaboost.py` | Ensemble Learning | Combines weak learners, reweighting misclassified samples each round |
| Support Vector Machine (SVM) | `Support_Vector_Machine.py` | Classification | Finds the maximum-margin hyperplane between classes |
| Naive Bayes | `naivebayes.py` | Classification | Applies Bayes' theorem assuming feature independence |
| K-Means Clustering | `kmeans.py` | Unsupervised Learning | Partitions data into k clusters by minimizing intra-cluster distance |
| Principal Component Analysis (PCA) | `pca.py` | Dimensionality Reduction | Projects data onto directions of maximum variance |
| Linear Discriminant Analysis (LDA) | `lda.py` | Dimensionality Reduction | Projects data to maximize class separability |
| Regression Utilities | `regression.py` | Utilities | Shared helper functions (metrics, base regression logic) |

Each implementation is self-contained, making it easy to read, study, modify, and experiment with individual algorithms.

---

## 📂 Project Structure

```
Machine-Learning-From-Scratch/
│
├── K-Nearest_Neighbors.py
├── Support_Vector_Machine.py
├── adaboost.py
├── decision_tree.py
├── kmeans.py
├── lda.py
├── linear_regression.py
├── logistic_regression.py
├── naivebayes.py
├── pca.py
├── perceptron.py
├── random_forest.py
├── regression.py
├── __init__.py
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/fares-ahmed7/Machine-Learning-From-Scratch.git
cd Machine-Learning-From-Scratch
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

---

## 🚀 Usage

Each algorithm can be imported and used independently. Example with Linear Regression:

```python
from linear_regression import LinearRegression
import numpy as np

X_train, y_train = ...  # your training data
X_test = ...

model = LinearRegression(learning_rate=0.01, n_iters=1000)
model.fit(X_train, y_train)
predictions = model.predict(X_test)
```

Example with K-Nearest Neighbors:

```python
from K_Nearest_Neighbors import KNN

model = KNN(k=3)
model.fit(X_train, y_train)
predictions = model.predict(X_test)
```

> Every implementation follows a familiar `fit()` / `predict()` interface inspired by scikit-learn, making it easy to switch between algorithms while keeping the learning process transparent.

---

## 🗺️ Roadmap

Planned additions to keep expanding the collection:

- [ ] Neural Network from scratch (feedforward + backpropagation)
- [ ] Gradient Boosting (simplified)
- [ ] Gaussian Mixture Models (GMM)
- [ ] Hierarchical Clustering
- [ ] Unit tests for each algorithm
- [ ] Jupyter notebooks with visualizations and dataset demos

Contributions toward any of these are very welcome — see [Contributing](#-contributing).

---

## 🎯 Project Goals

- Reinforce theoretical understanding by implementing algorithms from scratch
- Build intuition for the mathematics behind machine learning
- Keep implementations simple, readable, and dependency-light
- Provide educational reference implementations for students and self-learners
- Develop a stronger understanding before relying on production libraries such as scikit-learn and PyTorch

---

## 🛠️ Tech Stack

- **Language:** Python 3
- **Core library:** NumPy
- *(See `requirements.txt` for the full list of dependencies)*

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome!

1. Fork the repository
2. Create a new branch (`git checkout -b feature/algorithm-name`)
3. Commit your changes (`git commit -m 'Add XYZ algorithm'`)
4. Push to the branch (`git push origin feature/algorithm-name`)
5. Open a Pull Request

---

## 📚 References

This project is inspired by standard machine learning literature and educational resources, including:

- *Pattern Recognition and Machine Learning* — Christopher M. Bishop
- *The Elements of Statistical Learning*
- *Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow*
- Stanford CS229 Machine Learning Notes

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 👤 Author

**Fares Ahmed**
GitHub: [@fares-ahmed7](https://github.com/fares-ahmed7)

---

⭐ If you find this repository useful, consider giving it a star — it helps others discover it and supports its continued development.