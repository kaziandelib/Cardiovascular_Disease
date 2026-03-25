Machine learning project for predicting cardiovascular disease using clinical data, with feature engineering, model comparison, and performance evaluation.

# Cardiovascular Disease Prediction using Machine Learning

## 📌 Overview
This project develops an end-to-end machine learning pipeline to predict the presence of cardiovascular disease using clinical and lifestyle data. The workflow includes data cleaning, feature engineering, model training, evaluation, and interpretation.

---

## 📊 Dataset
- Source: Cardiovascular Disease dataset (70,000 records)
- Features include:
  - Demographics (age, gender)
  - Anthropometric data (height, weight)
  - Clinical measurements (blood pressure, cholesterol, glucose)
  - Lifestyle factors (smoking, alcohol, activity)

---

## 🧹 Data Preprocessing
- Removed physiologically implausible values (e.g., invalid blood pressure readings)
- Converted age from days to years
- Engineered **Body Mass Index (BMI)**
- Encoded categorical variables (one-hot and ordinal encoding)

---

## 🔍 Exploratory Data Analysis
- Distribution plots for numerical features
- Count plots for categorical features
- Correlation heatmap and pairplots
- Crosstab analysis for categorical relationships with target

---

## 🧠 Feature Selection
- Applied **Random Forest feature importance**
- Created datasets using thresholds:
  - Importance > 0.01
  - Importance > 0.03

---

## 🤖 Models Implemented
- Random Forest
- Gradient Boosting
- Multi-Layer Perceptron (MLP)
- Logistic Regression

---

## 📏 Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1 Score
- **F2 Score** (recall-focused)
- ROC-AUC

---

## 🔁 Validation Strategy
- Stratified train/validation/test split
- Stratified k-fold cross-validation (k=5)

---

## ⚙️ Hyperparameter Tuning
- Performed using **GridSearchCV**
- Optimised using **F2-score** to prioritise recall

---

## 📈 Model Interpretation
- ROC curves for model comparison
- Confusion matrices
- **Permutation feature importance**

---

## 🏁 Final Results
- Best models: Gradient Boosting and MLP
- ROC-AUC ≈ 0.79
- Consistent performance across feature thresholds
- Minimal performance drop with reduced feature set

---

## 🚀 Key Takeaways
- Data cleaning significantly improved model reliability
- Feature selection reduced complexity with little performance loss
- F2-score optimisation prioritised identifying high-risk patients

---

## 🛠️ Technologies Used
- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

---
