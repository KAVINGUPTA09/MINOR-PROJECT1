# 🩺 Diabetes Prediction Using Supervised Machine Learning

## 📌 Project Overview

Diabetes is one of the most common chronic diseases affecting millions of people worldwide. Early diagnosis can help patients receive timely treatment and reduce the risk of severe complications such as heart disease, kidney failure, nerve damage, and vision loss.

This project develops a **Supervised Machine Learning** model to predict whether a person is diabetic based on various medical attributes such as glucose level, blood pressure, BMI, insulin level, age, and other health-related factors. The model aims to assist healthcare professionals in making faster and more accurate preliminary diagnoses.

---

# 🎯 Objectives

The primary objectives of this project are:

* Collect a reliable diabetes dataset.
* Perform data preprocessing.
* Handle missing values and scale numerical features.
* Perform Exploratory Data Analysis (EDA).
* Train a supervised machine learning classification model.
* Evaluate model performance using classification metrics.
* Analyze results and identify possible improvements.

---

# 📂 Dataset

This project uses the **Pima Indians Diabetes Database**, a widely used healthcare dataset for binary classification problems.

### Dataset Information

* **Total Records:** 768
* **Input Features:** 8
* **Target Variable:** Outcome
* **Problem Type:** Binary Classification

### Input Features

| Feature                  | Description                      |
| ------------------------ | -------------------------------- |
| Pregnancies              | Number of pregnancies            |
| Glucose                  | Plasma glucose concentration     |
| BloodPressure            | Diastolic blood pressure (mm Hg) |
| SkinThickness            | Triceps skin fold thickness (mm) |
| Insulin                  | 2-Hour serum insulin             |
| BMI                      | Body Mass Index                  |
| DiabetesPedigreeFunction | Diabetes pedigree function       |
| Age                      | Age of the patient               |

### Target Variable

| Outcome | Meaning      |
| ------- | ------------ |
| 0       | Non-Diabetic |
| 1       | Diabetic     |

---

# 🛠 Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn

---

# ⚙️ Data Preprocessing

The following preprocessing steps were performed:

### 1. Import Libraries

* NumPy
* Pandas
* Matplotlib
* Scikit-learn

### 2. Load Dataset

The dataset was loaded into a Pandas DataFrame and inspected using:

* `head()`
* `info()`
* `describe()`
* `shape`

### 3. Handle Missing Values

Although no NULL values were present, several medical attributes contained **0 values**, which are medically invalid.

Affected features:

* Glucose
* BloodPressure
* SkinThickness
* Insulin
* BMI

These values were replaced using **Median Imputation**.

### 4. Remove Duplicates

Duplicate records were checked using:

```python
duplicated()
```

No duplicate records were found.

### 5. Feature Scaling

Numerical features were standardized using:

* `StandardScaler`

This ensures all features contribute equally during model training.

### 6. Train-Test Split

The dataset was divided into:

* **Training Set:** 80%
* **Testing Set:** 20%

---

# 📊 Exploratory Data Analysis (EDA)

EDA was performed before model training to better understand the dataset.

## Dataset Overview

Each row represents a patient, while each column represents a medical feature.

## Statistical Summary

The following statistical measures were analyzed:

* Mean
* Median
* Standard Deviation
* Minimum
* Maximum
* Quartiles

using:

```python
describe()
```

## Class Distribution

A count plot was generated to visualize diabetic and non-diabetic patient distribution.

## Correlation Analysis

A correlation heatmap was created to identify relationships among features.

## Feature Distribution

Histograms were plotted for all numerical variables to observe feature distributions.

## Box Plot Analysis

Box plots were used to detect outliers in:

* Glucose
* BMI
* Insulin
* BloodPressure

## Pairwise Relationship Analysis

Scatter plots were generated for important feature pairs:

* Glucose vs BMI
* Age vs Glucose
* BMI vs Insulin

---

# 🤖 Machine Learning Workflow

1. Data Collection
2. Data Preprocessing
3. Exploratory Data Analysis
4. Feature Scaling
5. Train-Test Split
6. Model Training
7. Model Evaluation
8. Performance Analysis

---

# 📈 Model Evaluation

The trained classification model can be evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* ROC-AUC Score

---

# 📁 Project Structure

```
Diabetes-Prediction/
│
├── dataset/
│   └── diabetes.csv
│
├── notebook/
│   └── Diabetes_Prediction.ipynb
│
├── README.md
│
└── requirements.txt
```

---

# 🚀 Future Improvements

* Hyperparameter tuning
* Feature engineering
* Cross-validation
* Deployment using Flask or Streamlit
* Integration with healthcare applications

---

# 📌 Conclusion

This project demonstrates the complete machine learning pipeline for predicting diabetes using supervised learning techniques. Data preprocessing and exploratory data analysis were performed to improve data quality and understand feature relationships before training the model. The resulting classification model can assist healthcare professionals in the early detection of diabetes and support preliminary medical decision-making.

---

# 👨‍💻 Author

**Kavin Gupta**

Minor Project

Bachelor of Technology (B.Tech)

Machine Learning
