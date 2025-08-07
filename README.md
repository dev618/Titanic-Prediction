# 🛠️ Titanic Survival Prediction  
*A Machine Learning Project using Logistic Regression*

## 📌 Objective
Predict whether a passenger survived the Titanic disaster using a **Logistic Regression** model trained on structured and cleaned data.

---

## 📂 Dataset Overview
The dataset contains demographic and travel information for passengers on the Titanic. The goal is to classify survival (`0` = No, `1` = Yes) based on these features.

---

## 🔍 Step 1: Data Import & Initial Exploration
- Loaded the dataset using **Pandas**
- Inspected structure using `.head()`, `.info()`, and `.describe()`
- Identified missing values and column types for cleaning

---

## 🧹 Step 2: Data Cleaning
- ❌ Dropped the `Cabin` column due to excessive missing values  
- 🧮 Filled missing `Age` values with the **mean age**  
- 📍 Filled missing `Embarked` values with the **mode** (most common port)

---

## 📊 Step 3: Exploratory Data Analysis (EDA)
Created visualizations to understand relationships between features and survival outcomes:
- **Sex vs Survival** 🚻
- **Pclass vs Survival** 🎫
- **Embarked vs Survival** ⚓

These charts helped in identifying the most influential features.

---

## 🔄 Step 4: Encoding Categorical Variables
- Converted categorical columns into numerical:
  - `Sex`: male → 0, female → 1  
  - `Embarked`: Converted to numeric codes
- Ensured all features were machine-learning-friendly

---

## 🧠 Step 5: Feature Selection & Data Splitting
- Removed irrelevant columns: `PassengerId`, `Name`, `Ticket`
- Split dataset:
  - **80% for training**
  - **20% for testing**

---

## 🤖 Step 6: Model Training & Evaluation
- Trained a **Logistic Regression** model on the cleaned training data  
- Made predictions on the test data  
- Evaluated model performance using **accuracy score**

---

## ✅ Final Outcome
A simple yet effective logistic regression model that can predict Titanic passenger survival based on well-preprocessed data. This project demonstrates the importance of:
- **Data cleaning**
- **Feature engineering**
- **Model evaluation**

---

## 📌 Tools & Libraries Used
- Python 🐍
- Pandas & NumPy 📊
- Matplotlib & Seaborn 📈
- Scikit-learn 🤖

---

## 📚 Future Improvements
- Add **cross-validation** for better model reliability  
- Try other models like **Random Forest** or **XGBoost**  
- Tune hyperparameters for better accuracy
