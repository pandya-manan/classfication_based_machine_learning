# Classification-based Machine Learning

This repository contains sample Jupyter Notebook files for all the key algorithms used in classification-based machine learning. Classification is a supervised learning technique where the goal is to predict the categorical class labels of new instances based on past observations.

## 📚 Algorithms Covered

The following classification algorithms are included in this repository:

- **Decision Tree** – A tree-based model that splits data into subsets based on feature values.
- **Logistic Regression (Binary Classification)** – Used when the target variable has two possible outcomes (e.g., Yes/No, 0/1).
- **Logistic Regression (Multi-class Classification)** – An extension of logistic regression for targets with three or more unordered categories.
- **Naive Bayes** – A probabilistic classifier based on Bayes' theorem, assuming feature independence.

## 📖 Algorithm Overview

| Algorithm | Type | Best Used When |
|-----------|------|----------------|
| Decision Tree | Tree-based | Interpretability is important, data has non-linear relationships |
| Logistic Regression (Binary) | Linear | Two-class problems with linear decision boundary |
| Logistic Regression (Multi-class) | Linear | More than two classes, linear separability |
| Naive Bayes | Probabilistic | High-dimensional data (e.g., text classification), independence assumption holds approximately |

## 🧪 Sample Code Snippet

Here's an example of binary logistic regression using `scikit-learn`:

```python
from sklearn.linear_model import LogisticRegression
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score

# Assuming X and y are your features and labels
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)

model = LogisticRegression()
model.fit(X_train, y_train)

predictions = model.predict(X_test)
print(f"Accuracy: {accuracy_score(y_test, predictions):.2f}")
```
## Author : Manan Pandya
