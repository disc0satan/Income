# Adult Income Prediction – Comparative Machine Learning Study

This project presents a comparative analysis of supervised and unsupervised machine learning techniques to predict whether an individual's annual income exceeds $50K using UCI Adult Census dataset.

The objective was to evaluate multiple learning algorithms and determine which model best captures the complex socioeconomic patterns influencing income levels.

---

## 📊 Problem Statement

Given demographic and socioeconomic features such as education, occupation, marital status, and working hours, the goal is to classify individuals into:

- Income ≤ 50K
- Income > 50K

The dataset presents key challenges including:
- High-cardinality categorical variables
- Class imbalance (majority ≤50K class)
- Skewed numerical distributions

---

## 🛠️ Tech Stack

- Python 3.x
- NumPy
- Pandas
- scikit-learn
- Matplotlib
- Seaborn

---

## ⚙️ Machine Learning Pipeline

### 1️⃣ Data Preprocessing
- Categorical feature encoding
- Z-score normalization using `StandardScaler`
- 80/20 train-test split
- Handling class imbalance through metric selection (F1, AUC)

### 2️⃣ Models Implemented

- K-Nearest Neighbors (KNN)
- Decision Tree (Gini Impurity)
- Multi-Layer Perceptron (MLP Neural Network)
- K-Means Clustering (k=2)

---

## 📈 Model Performance

| Model                  | Accuracy | F1-Score | AUC  |
|------------------------|----------|----------|------|
| KNN                    | 0.82     | 0.79     | 0.78 |
| Decision Tree          | 0.81     | 0.76     | 0.75 |
| MLP (Neural Network)   | 0.85     | 0.83     | 0.88 |

The Multi-Layer Perceptron (MLP) achieved the highest performance, demonstrating strong capability in modeling non-linear relationships within high-dimensional socioeconomic data.

---

## 🔍 Key Insights

- Education level showed the strongest correlation with income.
- Class imbalance significantly affected accuracy metrics.
- Neural networks captured complex feature interactions better than instance-based and rule-based models.
- K-Means clustering revealed that income groups do not perfectly align with demographic clusters.

---

## 🚀 Future Improvements

- Apply SMOTE for minority class oversampling
- Hyperparameter tuning using GridSearchCV
- Explore ensemble models (Random Forest, Gradient Boosting)

---

## 👥 Contributors

- Jannatul Ferdous
- Md. Fardin Islam Mahi

---

## 📚 Course Context

This project was developed as part of the CSE422 Machine Learning Lab course at BRAC University.
