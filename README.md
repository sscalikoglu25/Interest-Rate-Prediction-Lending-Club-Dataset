# LendingClub Interest Rate Prediction

## Overview

This project develops machine learning models to predict loan interest rates using a modified version of the LendingClub dataset, which includes only variables available at the time of loan origination. The goal is to understand the key drivers of loan pricing and evaluate how accurately interest rates can be predicted using borrower and loan characteristics.

---

## Dataset

* Source: LendingClub (modified dataset provided for academic use)
* File: `LC_HW2.csv`
* Scope: Loan origination features only (no post-origination data)

The dataset includes borrower financial information, loan attributes, and credit-related variables used by lenders to determine interest rates.

---

## Objectives

* Preprocess and clean the dataset for modeling
* Train and compare multiple machine learning models to predict loan interest rates
* Evaluate model performance using appropriate regression metrics
* Apply model explainability techniques to interpret predictions and identify key drivers of interest rates

---

## Methodology

### Data Preprocessing

* Handled missing values and outliers
* Encoded categorical variables
* Scaled numerical features where appropriate
* Split data into training and testing sets

### Models Implemented

The following supervised learning models from scikit-learn were trained and compared:

* Regression Tree
* Random Forest

### Model Evaluation

Models were evaluated using:

* Root Mean Squared Error (RMSE)
* Mean Absolute Error (MAE)
* R-squared (R²)

---

## Results

* The Random Forest model achieved the strongest predictive performance, capturing non-linear relationships in the data.
* Tree-based methods generally outperformed linear and kernel-based models in this setting.
* Model performance highlights the importance of borrower risk characteristics and loan structure in determining interest rates.

---

## Model Explainability

To interpret model predictions and provide transparency:

* **Feature Importance (Random Forest):** Identified the most influential variables driving interest rate predictions
* **Partial Dependence Plots:** Marginal effect of individual features to model predictions holding everything else constant

### Key Insights

* Credit-related variables (e.g., credit score, debt-to-income ratio) are strong predictors of interest rates
* Loan characteristics (e.g., term, loan amount) also significantly influence pricing
* The model captures meaningful patterns consistent with real-world lending practices

---

## Tools & Technologies

* Python
* pandas, numpy
* scikit-learn
* matplotlib, seaborn
  

---

## Conclusion

This project demonstrates how machine learning can be applied to model loan pricing and uncover the factors that influence interest rates. By combining predictive modeling with explainability techniques, the analysis provides both accurate predictions and actionable insights into lending decisions.

---

## Future Improvements

* Hyperparameter tuning for improved model performance
* Testing additional models (e.g., gradient boosting)
* Incorporating external macroeconomic variables
* Expanding explainability with SHAP (SHapley Additive exPlanations)

---
