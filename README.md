# Exploratory Data Analysis (EDA) for Data Science and Machine Learning

## Overview
This repository contains the work from my recent IBM Guided Project focused on Exploratory Data Analysis (EDA) and Data Preprocessing for Machine Learning. The project demonstrates a systematic approach to analyzing, cleaning, and preparing data for predictive modeling, specifically focusing on a regression task using the `sklearn` Diabetes dataset.

## Objectives
The primary goal of this project was to learn and apply essential EDA and data preprocessing techniques to improve the performance of machine learning models. 

Key objectives included:
* Interpreting key EDA plots and statistics.
* Performing basic feature engineering.
* Detecting and handling missing data and outliers.
* Improving a prediction model by using insights obtained through EDA.

## Skills & Techniques Learned
Throughout this project, I gained hands-on experience with the following techniques:

### 1. Initial Data Preprocessing
* **One-Hot Encoding:** Converting categorical variables (like `sex`) into numerical indicator columns using `sklearn.preprocessing.OneHotEncoder` to prevent the model from misinterpreting categorical hierarchies.
* **Train-Test Splitting:** Partitioning the dataset into training (67%) and testing (33%) sets using `train_test_split` to ensure models are evaluated on unseen data.

### 2. Exploratory Data Analysis (EDA)
* **Descriptive Statistics:** Utilizing `pandas` functions like `head()`, `tail()`, and `describe()` to understand data distributions, standard deviations, means, and identify potential anomalies or outliers.
* **Visualizing Data:** Using libraries like `seaborn` and `fasteda` to create histograms, boxplots, correlation matrices, and pair plots to uncover feature relationships.

### 3. Missing Data Analysis & Imputation
* **Missing Data Visualization:** Using the `missingno` library to create missing value matrices and sparklines, allowing for the visual detection of whether data is missing at random or in systematic patterns.
* **Imputation Strategies:** Comparing the impact of different missing data handling techniques on model performance:
    * Dropping missing observations entirely.
    * Mean imputation using `sklearn.impute.SimpleImputer`.
    * Median imputation using `sklearn.impute.SimpleImputer` (which proved robust against extreme values).
* **Baseline Evaluation:** Building baseline Linear Regression models to evaluate how different missing-data imputation strategies affect the Root Mean Squared Error (RMSE).

## Tools & Libraries Used
* **Python**
* **Data Manipulation:** `pandas`, `NumPy`
* **Machine Learning:** `scikit-learn` (`LinearRegression`, `SimpleImputer`, `OneHotEncoder`, `train_test_split`, `root_mean_squared_error`)
* **Data Visualization:** `seaborn`, `Matplotlib`, `missingno`, `fasteda`

## Acknowledgments
* **IBM** for providing the guided project curriculum and learning environment.
