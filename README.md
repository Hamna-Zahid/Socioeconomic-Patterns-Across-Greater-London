
# README: Analysis of Economic, Demographic, and Social Issues in Greater London MSOAs

## Overview

This project investigates the relationships between economic, demographic, and social indicators across Middle Layer Super Output Areas (MSOAs) in Greater London. The analysis uses various statistical techniques and models to understand factors influencing median house prices and urban characteristics.

---

## Dataset Summary

The dataset includes the following variables:

- Median house prices
- Population density
- Working-age population percentage
- Life expectancy
- Ethnic composition (BAME %)
- Unemployment rate
- Median household income
- Car ownership per household
- Property ownership rate
- Annual house sales volume
- Area classification as Inner or Outer London

---

## Statistical Methods Used

### 1. Exploratory Data Analysis (EDA)

Key findings:
- Positive correlations: Median house prices are positively linked with population density, working age %, life expectancy, and income.
- Negative correlations: Unemployment rate vs. household income, BAME vs. OwnershipRate, WorkingAge vs. CarPerHH.
- Observations: Economic and demographic variables are interrelated with housing affordability and ownership disparities.

### 2. Simple Linear Regression (SLR)

**Dependent Variable**: Median House Price (MedianHP)  
**Covariate**: Median Household Income (MedianHHIncome)

- Projection: MedianHP increases from ~£226,040 (lowest income quartile) to ~£384,122 (highest income quartile).
- Interpretation: Income is a significant determinant of housing prices.

### 3. Multiple Linear Regression (MLR)

**Dependent Variable**: Median House Price  
**Covariates**: Median Household Income, Ownership Rate, and House Sales

- Predicted MedianHP:
  - Lower Quartile: ~£230,043
  - Median: ~£276,308
  - Upper Quartile: ~£208,904
- Insight: Multiple variables together provide a more nuanced view of housing price determinants.

### 4. Logistic Regression (LR)

**Outcome Variable**: Inner (binary: Inner London = 1, Outer London = 0)  
**Predictor**: Median House Price

- Chi-squared statistic = 81.46, p-value < 0.001 (model is statistically significant)
- Log-likelihood = -621.96; Pseudo R² = 0.0615
- Odds Ratio for MedianHP = 1.000004 (minimal practical effect)
- Conclusion: Although statistically significant, MedianHP alone has limited predictive power for Inner/Outer classification.

---

## Summary

This analysis highlights:
- How economic variables such as income and unemployment influence housing prices.
- The complexity of modeling urban housing dynamics.
- The limited practical utility of single-variable models in classification problems like Inner vs. Outer London.

---

## Requirements

- Stata for statistical analysis
- Markdown or Jupyter for report presentation

---

## How to Use

1. Review the EDA summary to identify key trends.
2. Refer to SLR and MLR sections for insights on predicting house prices.
3. Use LR outcomes for classification modeling between Inner and Outer London.
4. Apply findings to inform urban planning and housing policy decisions.

---

## Authors

- Analysis by: Hamna Zahid
- Prepared with: Stata
