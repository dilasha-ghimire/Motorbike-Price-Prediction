# Motorbike Price Prediction Using Machine Learning

## Overview

This project analyzes a **European Motorbike Marketplace** dataset to understand **factors influencing motorbike prices** and to build a **machine learning model** capable of predicting prices based on key features.

The workflow combines **exploratory data analysis (EDA)** with **supervised machine learning**, focusing on data cleaning, feature selection, and model evaluation. The analysis is implemented in **Python** using a **Jupyter Notebook**.

---

## Dataset

**File:** `europe-motorbikes-zenrows.csv`  
**Source:** Kaggle – Motorbike Marketplace Dataset  
**Domain:** Online motorbike listings across Europe

The dataset contains structured information about motorbike listings, including technical specifications and pricing.

**Key features include:**

- **Price** – Listing price of the motorbike (target variable)
- **Mileage** – Distance traveled
- **Power** – Engine power
- **Fuel Type** – Petrol, diesel, electric, etc.
- **Gear Type** – Manual or automatic
- **Offer Type** – Dealer or private seller

---

## Project Files

- `notebook.ipynb` – Jupyter notebook containing EDA, preprocessing, and machine learning model implementation
- `europe-motorbikes-zenrows.csv` – Dataset used for analysis
- `README.md` – Project documentation

---

## Tools and Technologies

**Language:** Python 3  
**Environment:** Jupyter Notebook

### Libraries Used

- `pandas` – Data loading, cleaning, and manipulation
- `numpy` – Numerical computations
- `matplotlib` – Data visualization
- `seaborn` – Statistical plots for EDA
- `scikit-learn` – Machine learning modeling and evaluation

---

## Work Conducted

### 1. Data Import and Exploration

- Loaded the dataset into a pandas DataFrame.
- Inspected data structure, column types, and summary statistics.
- Identified the target variable (**price**) and relevant predictors.

### 2. Data Cleaning and Preprocessing

- Checked for missing values and data consistency.
- Detected and removed price outliers using the **IQR method** to improve data quality.
- Selected relevant numerical and categorical features for modeling.
- Encoded categorical variables using preprocessing techniques.
- Split the dataset into **training and testing sets**.

### 3. Exploratory Data Analysis (EDA)

- Visualized price distribution using boxplots.
- Analyzed the effect of mileage and power on motorbike prices.
- Observed skewness and variability in pricing due to extreme values.
- Compared price behavior before and after outlier removal.

### 4. Machine Learning Model

- Implemented a **Linear Regression** model to predict motorbike prices.
- Trained the model using selected features:
  - Mileage
  - Power
  - Fuel type
  - Gear type
  - Offer type
- Generated predictions on the test dataset.

### 5. Model Evaluation

- Evaluated model performance using:
  - **Mean Absolute Error (MAE)**
  - **R² Score**
- Visualized actual vs. predicted prices using a scatter plot.
- Assessed model limitations due to linear assumptions and feature complexity.

---

## Key Findings / Conclusions

- **Mileage and Power** are strong indicators of motorbike price.
- **Categorical features** such as fuel type and offer type contribute to price variation.
- **Outlier removal** significantly improves data interpretability and model stability.
- **Linear Regression** provides a reasonable baseline but struggles with highly non-linear pricing patterns.
- More advanced models (e.g., tree-based or ensemble methods) could further improve prediction accuracy.

This project demonstrates a complete **end-to-end machine learning pipeline**, from raw data exploration to predictive modeling and evaluation.

---

## References

- Kaggle: Motorbike Marketplace Dataset  
  https://www.kaggle.com/datasets/mexwell/motorbike-marketplace/data/
