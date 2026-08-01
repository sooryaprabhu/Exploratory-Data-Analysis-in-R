# USED CAR PRICE PREDICTION — EDA & LINEAR REGRESSION

University assessment project analysing used car prices using 
Exploratory Data Analysis and Linear Regression in R.

---

## PROJECT OVERVIEW

Analysed a dataset of 409 used cars with 16 features to predict 
selling price using statistical analysis and machine learning.

---

## WHAT WAS DONE

**Data Cleaning:**
- Handled 138 missing values (33% of dataset)
- Median imputation for skewed continuous variables
- Mode imputation for binary variables
- Winsorizing method for outlier treatment
- Fixed fuel type spelling errors (Petrol/Pertol)

**Exploratory Data Analysis:**
- Univariate analysis (mean, median, mode, std)
- Bivariate analysis (price vs brand, fuel, transmission)
- Correlation matrix analysis
- Welch Two Sample t-test for damaged vs non-damaged cars
- Statistical hypothesis testing

**Key Findings:**
- Petrol cars dominate the dataset (94%)
- Automatic transmission cars sell at higher prices (93.4%)
- Year has highest positive correlation with price
- Mileage has highest negative correlation with price
- Damaged cars sell at significantly lower prices

**Modelling:**
- Linear Regression (70/30 train/test split)
- Initial model: R²=0.73, RMSE=7,286
- Improved model (Cook's distance outlier removal): R²=0.75

---

## TECH STACK

![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)

**Libraries:** tidyverse · ggplot2 · caret · lmtest · plotly · 
dplyr · Hmisc · skimr · rstatix · pROC

---

## RESULTS

| Model | R² | Adjusted R² | RMSE |
|-------|-----|-------------|------|
| Linear Regression | 0.736 | 0.722 | 7,286 |
| Improved (Cook's D) | 0.752 | 0.742 | Lower |

---

## ACADEMIC CONTEXT

**Module:** Data Science & Analytics
**Institution:** Brunel University London
**Author:** Soorya Prabhu

---

## FILES

```
├── EDA_Car_Price.Rmd    # Main R Markdown file
├── subsetted_data-1.csv # Dataset
└── README.md
```
