# 🏥 Patient Health Data Cleaning & Preprocessing Project

## 📌 Project Overview

This project focuses on **data cleaning and preprocessing** of a healthcare dataset containing patient information such as age, BMI, cholesterol, glucose, gender, and region.

The main objective is to prepare high-quality data by handling:

* Missing values
* Outliers
* Data inconsistencies

---

## 🎯 Objectives

* Identify and treat missing values using appropriate techniques
* Detect outliers using statistical methods (Z-score & IQR)
* Handle extreme values using Winsorization
* Compare dataset before and after preprocessing

---

## 📂 Dataset Description

The dataset contains patient health-related attributes:

* `age` → Patient age
* `bmi` → Body Mass Index
* `blood_pressure` → Blood pressure levels
* `cholesterol` → Cholesterol level
* `glucose` → Glucose level
* `gender` → Male/Female
* `region` → Geographic region

---

## 🛠️ Tools & Libraries Used

* Python 🐍
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* SciPy

---

## 🔄 Project Workflow

### 1️⃣ Data Loading

* Loaded dataset using Pandas
* Created a copy to preserve original data

---

### 2️⃣ Data Exploration

* Used `.info()` and `.describe()`
* Checked missing values and distributions
* Visualized data using histograms

---

### 3️⃣ Missing Value Handling

* **Numerical columns:**

  * Age → Mean Imputation
  * BMI, Cholesterol, Glucose → Median Imputation

* **Categorical columns:**

  * Used **Random Imputation** to preserve distribution

---

### 4️⃣ Advanced Imputation (Optional)

* KNN Imputer
* MICE (Iterative Imputer)

---

### 5️⃣ Outlier Detection

* **Z-score Method**

  * Used for detecting extreme values in cholesterol and glucose

* **IQR Method**

  * Used for identifying unusual BMI values

---

### 6️⃣ Outlier Treatment

* Applied **Winsorization (1st & 99th percentile)**
* Capped extreme values instead of removing rows

---

### 7️⃣ Comparison (Before vs After)

* Dataset shape remained unchanged
* Summary statistics improved:

  * Reduced max/min extremes
  * Lower standard deviation

---

### 8️⃣ Visualization

* Boxplots used to compare:

  * Before outlier handling
  * After winsorization

---

## 📊 Key Results

* Missing values successfully handled
* Outliers detected and controlled
* Data distribution improved
* No data loss (rows preserved)

---

## 🧠 Key Learnings

* Missing values and outliers are **different problems**
* Winsorization is better than removal for healthcare data
* Maintaining original dataset is critical
* Proper pipeline structure avoids confusion

---

## 📁 Output

* Cleaned dataset saved as:

  ```
  cleaned_dataset.csv
  ```

---

## 🚀 Future Scope

* Apply machine learning models
* Feature engineering
* Predict patient health risks

---


## 📌 Conclusion

This project demonstrates a complete data preprocessing pipeline using industry-relevant techniques. The final dataset is clean, consistent, and ready for further analysis or modeling.

---
