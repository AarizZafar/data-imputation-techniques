
# 🧩 Data Imputation Techniques

This repository contains a collection of notebooks demonstrating various methods to handle missing data in datasets. Missing data is a common issue in real-world data science and machine learning workflows. How you deal with it can significantly impact model accuracy and insight quality.

---

## 📌 What is Missing Data?

Missing data occurs when no value is stored for a variable in an observation. It can arise due to errors in data collection, equipment malfunction, manual entry mistakes, or data corruption.

### ❗ Why is it a problem?

- It can bias results if not handled correctly
- Reduces statistical power
- Most ML models do not support missing values directly
- Can distort distributions and relationships among variables

---

## 🔧 Techniques Covered

| Technique Name                     | File Name                            | Description |
|-----------------------------------|--------------------------------------|-------------|
| Arbitrary Value Imputation        | `arbitrary_value_imputation.ipynb`   | Replaces missing values with a fixed arbitrary value (e.g., -999 or 0) |
| Auto Imputer Parameter Selection  | `auto_imputer_parameter_selection.ipynb` | Demonstrates how to automatically select imputer parameters using GridSearch or scoring |
| Complete Case Analysis (CCA)      | `complete_case_analysis_cca.ipynb`   | Removes rows with any missing value |
| Iterative Imputer                 | `iterative_imputation.ipynb`         | Uses multivariate regression-based imputation iteratively |
| KNN Imputer                       | `knn_imputation.ipynb`               | Imputes based on values from nearest neighbors |
| Categorical Handling              | `missing_categorical_handling.ipynb` | Covers mode imputation, "missing" label, and category-specific tricks |
| Missing Indicator                 | `missing_value_indicator.ipynb`      | Adds a boolean column indicating where data was missing |
| Random Sample Imputation          | `random_sample_imputation.ipynb`     | Fills missing values by randomly sampling existing values from the column |
| Simple Imputer (Mean/Median)     | `simple_imputation_mean_median.ipynb`| Fills missing values using mean or median of the column |

---

## ✅ When to Use What?

| Technique                 | Advantage                                            | Disadvantage |
|--------------------------|------------------------------------------------------|--------------|
| Complete Case Analysis   | Simple, no modeling involved                        | Can lose too much data |
| Arbitrary Value          | Easy to implement                                   | May distort distribution |
| Mean/Median Imputation   | Fast and good for numerical data                    | Ignores feature relationships |
| Random Sample            | Maintains distribution                              | Adds randomness |
| Missing Indicator        | Useful with other imputations                       | Alone, it doesn’t solve missingness |
| Categorical Labeling     | Keeps category structure intact                     | Adds artificial categories |
| KNN Imputer              | Uses similarity for accurate filling                | Computationally expensive |
| Iterative Imputer        | Captures feature relationships                      | Slow, can overfit |
| Auto Parameter Tuning    | Finds optimal strategy automatically                | More complex setup |

---

## 📁 Structure

- `Data_set/` – contains sample datasets with missing values
- `Images/` – generated plots or diagrams
- Individual `.ipynb` notebooks – each demonstrates one imputation technique

---



