# diabetesassignment
# Diabetes Dataset Analysis and Preprocessing

## Project Overview

This project focuses on data cleaning, preprocessing, outlier handling, feature engineering, and feature scaling using a Diabetes Dataset. The analysis was performed using Python libraries such as Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn.

The goal of this project is to prepare high-quality healthcare data for machine learning and statistical analysis.

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

# Dataset

Dataset Source:

```python
https://raw.githubusercontent.com/GeethaGunasekaran1/Dataset_rep/refs/heads/main/diabetes.csv
```

---

# Project Tasks

## Task 1 – Data Loading & Inspection

* Loaded dataset using Pandas
* Displayed:

  * head()
  * tail()
  * shape
  * columns
  * info()
  * dtypes
* Identified:

  * Numerical columns
  * Categorical columns

---

## Task 2 – Data Cleaning

### Column Renaming

Renamed columns for better readability:

* ID → Visit_ID
* No_Pation → Patient_ID

### Categorical Value Checking

Validated categorical values:

* Gender:

  * F → Female
  * M → Male
* CLASS:

  * N → No Diabetes
  * P → Pre-diabetes
  * Y → Diabetes

### Statistical Analysis

Generated:

* Mean
* Median
* Standard Deviation
* Minimum Values
* Maximum Values

### Missing Value Handling

* Numerical columns → Median Imputation
* Categorical columns → Mode Imputation

### Duplicate Removal

* Identified duplicate rows
* Removed duplicates

### Data Visualization

* Created boxplots for numerical columns
* Analyzed distributions and outliers

---

# Task 3 – Outlier Handling

## Retained Outliers

Outliers were retained in:

* AGE
* HbA1c
* BMI

Reason:
These medical values may represent genuine diabetic conditions and are clinically important.

## Filtered Outliers

Used percentile filtering:

* Cr column → Removed values above 99.5 percentile
* Urea column → Removed values above 99.9 percentile

## Removed Extreme Lipid Outliers

Applied IQR method on:

* LDL
* HDL
* VLDL
* TG
* Chol

---

# Task 4 – Data Transformation

## Feature Engineering

Applied Label Encoding on:

* Gender column

## Feature Scaling

Applied Standardization using StandardScaler on:

* AGE
* BMI
* Cr

Reason:
Standardization improves model performance by ensuring all features contribute equally.

---

# Project Structure

```python
├── diabetes_analysis.ipynb
├── cleaned_diabetes_dataset.csv
├── README.md
└── requirements.txt
```

---

# Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/diabetes-data-analysis.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# Run the Project

```bash
python diabetes_analysis.py
```

or open the Jupyter Notebook:

```bash
jupyter notebook
```

---

# Sample Output

* Cleaned Dataset
* Boxplots
* Missing Value Reports
* Encoded Features
* Scaled Numerical Features

---

# Learning Outcomes

Through this project, I learned:

* Data Cleaning Techniques
* Missing Value Imputation
* Outlier Detection & Removal
* Feature Engineering
* Feature Scaling
* Exploratory Data Analysis (EDA)
* Healthcare Data Preprocessing

---

# Future Improvements

* Machine Learning Model Building
* Diabetes Prediction System
* Interactive Dashboard
* Deployment using Streamlit or Flask

---

# Author

Mohamed Liyakath Ali

B.Tech Artificial Intelligence and Data Science

GitHub:
https://github.com/Mohamedliyakathali

LinkedIn:
https://www.linkedin.com/in/mohamed-liyakath-ali

```
```
