# 💳 Credit Card Fraud Detection using Machine Learning

## 📌 Project Overview

This project focuses on detecting fraudulent credit card transactions using machine learning models.

The dataset contains anonymized transaction features (`V1–V28`) obtained through PCA transformation, along with:
- `Time`
- `Amount`
- `Class` (Target variable)

Where:
- 0 → Not Fraud
- 1 → Fraud

The main challenge of this dataset is **extreme class imbalance**.

---

## 📊 Dataset Information

- Total Transactions: 284,807
- Total Features: 31
- Fraudulent Transactions: 492
- Non-Fraud Transactions: 284,315

### ⚠️ Class Distribution

- Non-Fraud → 99.83%
- Fraud → 0.17%

This makes the dataset highly imbalanced.

---

## 🔍 Data Exploration

### ✔ Checked for:
- Missing values → None found
- Data types → Verified
- Statistical summary → Analyzed using `describe()`
- Correlation matrix → Visualized using heatmap

### 📈 Visualizations Performed
- Bar plot for class distribution
- Full correlation heatmap
- Fraud percentage analysis

---

## ⚖️ Problem: Class Imbalance

Fraudulent transactions represent only:


::contentReference[oaicite:0]{index=0}


of the dataset.

Because of this imbalance, **accuracy alone is not a reliable metric**.

---

## 🤖 Models Used

For demonstration, only the `Amount` feature was used for training.

### 1️⃣ Logistic Regression

Logistic Regression predicts probability using the sigmoid function:


::contentReference[oaicite:1]{index=1}


Where:
- p = probability of fraud
- z = weighted sum of input features

### Steps:
- Train-Test Split (80-20)
- Feature Scaling using StandardScaler
- Model Training
- Prediction
- Accuracy Evaluation

📊 Accuracy: **99.83%**

---

### 2️⃣ Random Forest Classifier 🌲

An ensemble model that builds multiple decision trees.

Steps:
- Feature Scaling
- Model Training
- Prediction
- Accuracy Evaluation

📊 Accuracy: **99.80%**

---

## 📊 Model Comparison

| Model                  | Accuracy |
|-------------------------|----------|
| Logistic Regression     | 99.83%   |
| Random Forest           | 99.80%   |

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🎯 Conclusion

- The dataset is extremely imbalanced.
- Both models achieved high accuracy.
- However, deeper evaluation is required for real-world fraud detection.
- Model improvement should focus on minority class prediction.

---

⭐ *"Detecting fraud before it costs millions."*
