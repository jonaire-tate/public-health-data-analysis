# Public Health Data Analysis

A two-level exploratory and predictive analysis of diabetes prevalence in the United States, examining both state-level socioeconomic factors and individual-level health indicators.

## Overview

This project investigates what drives geographic variation in U.S. diabetes prevalence. Analysis operates at two complementary levels: the state/county level using demographic and economic data, and the individual level using CDC behavioral survey data.

## Research Questions

- Are higher poverty rates, lower income per capita, and larger proportions of older adults associated with higher state-level diabetes prevalence?
- Which individual-level behavioral and health indicators best predict a diabetes diagnosis?

## Data Sources

- [Kaiser Family Foundation – Adults with Diagnosed Diabetes by State](https://www.kff.org/state-health-policy-data/state-indicator/adults-with-diabetes-by-age/)
- [U.S. Census Bureau – American Community Survey via Kaggle](https://www.kaggle.com/datasets/muonneutrino/us-census-demographic-data)
- [CDC BRFSS 2015 Diabetes Health Indicators – Kaggle](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset)

## Methods

- Univariate and bivariate exploratory analysis
- PCA (PC1 explains 71.1% of ACS variance)
- Random Forest Classifier with GridSearchCV (test AUC = 0.825)
- Correlation heatmaps and feature importance analysis

## Key Findings

- Poverty rate showed the strongest correlation with state-level diabetes prevalence (r = 0.79)
- Income per capita showed a moderate negative correlation (r = -0.51)
- Top individual-level predictors: general health status, BMI, age, and high blood pressure
- Behaviorally modifiable variables (physical activity, smoking) ranked low once dominant features were controlled for

## Tools Used

Python, pandas, scikit-learn, matplotlib, seaborn, Jupyter Notebook
