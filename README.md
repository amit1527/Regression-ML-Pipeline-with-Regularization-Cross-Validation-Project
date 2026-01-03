# Regression-ML-Pipeline-with-Regularization-Cross-Validation-Project

This project implements an **end-to-end regression-based machine learning pipeline** to analyze and predict forest fire behavior using the **Algerian Forest Fires Dataset**.  
The workflow covers everything from raw data preprocessing to **cross-validated model selection**, with a strong focus on **regularization and generalization**.

---

## Dataset Overview

- **Dataset**: Algerian Forest Fires Dataset  
- **Regions**:
  - Bejaia Region
  - Sidi-Bel Abbes Region  
- The dataset contains meteorological and fire-related attributes recorded across different months.

---

## Project Structure

The project is divided into **four major stages**:

---

## 1️. Data Cleaning

Preprocessing steps applied to make the data model-ready:

- Encoded regions into a binary numerical feature  
  - `Bejaia Region → 0`  
  - `Sidi-Bel Abbes Region → 1`
- Removed missing and null values
- Cleaned column names by removing extra whitespaces
- Converted object-type columns into appropriate **integer and float** data types

---

## 2️. Exploratory Data Analysis (EDA)

Performed detailed analysis to understand feature behavior and relationships:

- Dropped unnecessary and redundant columns
- Encoded categorical class labels
- Visualized feature distributions using:
  - Histograms
  - Density plots
  - Pie charts
- Generated **correlation heatmaps** to analyze feature dependencies
- Conducted **month-wise and region-wise fire analysis** using count plots

---

## 3️. Model Training

Built and evaluated multiple regression models:

- Defined **independent (X)** and **dependent (y)** variables
- Performed **train–test split**
- Analyzed feature correlations using Seaborn
- Implemented a custom function to identify **features highly correlated with the target**
- Applied **feature scaling / standardization** to handle differing units and improve numerical stability

### Regression Models Used:
- Linear Regression  
- Ridge Regression  
- Lasso Regression  
- Elastic Net Regression  

### Evaluation Metrics:
- Mean Squared Error (MSE)
- R² Score

---

## 4️. Hyperparameter Tuning & Cross-Validation

Improved model robustness and generalization through:

- Cross-validated hyperparameter tuning using:
  - `LassoCV`
  - `RidgeCV`
  - `ElasticNetCV`
- Compared models using **MSE and R² score** after tuning
- Reduced overfitting and improved out-of-sample performance

---

## Key Takeaways

- Feature scaling is critical for regression models sensitive to magnitude differences
- Regularization techniques help mitigate **multicollinearity and overfitting**
- Cross-validation provides more reliable performance estimates than a single train–test split
- Correlation-based feature analysis improves interpretability and model selection

---

## Technicals used

- Python
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-learn
- Jupyter notebook 


## Contributing

Contributions and suggestions are welcome.  
Feel free to fork the repository or raise an issue.
