# Australian Real State Price Predicction

## Table of Contents

- [Table of Contents](#table-of-contents)
- [Introduction](#introduction)
  - [Methods Used](#methods-used)
  - [Technologies](#technologies)
- [Download and Setup](#download-and-setup)
  - [Prerequisites](#prerequisites)
  - [How to Run](#how-to-run)
- [Problem Statement](#problem-statement)
  - [Business Goal](#business-goal)
  - [Data Preparation:](#data-preparation)
  - [Model Building \& Evaluation](#model-building--evaluation)
  - [Conclusions](#conclusions)
    - [Ridge Regression](#ridge-regression)
    - [Lasso Regression](#lasso-regression)
    - [Most Significant Variables are:](#most-significant-variables-are)

### Introduction

This repository contains colab ipyn code that intends to predict house princing on Australian Real State market, the data is provided on data.csv file and also the file data_description.txt contains information about the columns defined in data.csv.

This project was created during the class of Machine Learnig of the DataScience Master of the Catholic University

### People Involved in the project
  -  Alicia Zamorano zamoranoalicia@gmail.com
  -  César Quiroga cesar.a.quiroga.c@gmail.com
  -  Juan Carlos Peralta juancarlosperaltaolivera@gmail.com
  -  Nilton Apaza nilton.apcon@gmail.com


### Methods Used
- Ridge Regression
- Lasso Regression

### Technologies
* Python
* Pandas
* Numpy
* Sklearn
* Google colab

## Download and Setup
### Prerequisites

This project can be run using colab.research from google https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwi906nQ3JP9AhVZHbkGHbsSCSIQFnoECA8QAQ&url=https%3A%2F%2Fcolab.research.google.com%2F&usg=AOvVaw3A5aPK2kLFzKOzb6sOckVw or anaconda navigator

### How to Run

You can download the source code cloning this repository using Git:

1. Open your favorite Terminal app (Unix, Linux or Macos), such as Terminal, Command, Console, iTerm2, so on.

2. Clone the repository

```
git clone <GITHUB_REPO_URL>
```

3. Open the ** *.ipynb** notebook file in Anaconda.

```
jupyter notebook <MDSv3_ML_P1Advanced_Regression.ipynb>
```

### Data Preparation:

1. Data Clearning and Missing Data Analysis.
2. Outlier Analysis & Treatment.
3. Deriving Categorical Columns.
4. Univariate Analysis.
5. Bivariate Analysis.
6. Multivariate Analysis.

### Model Building & Evaluation

1. Training and Test data split.
2. Feature Scaling - StandardScaler.
3. Feature Engineering & Selection using RFE and Variance Inflation factor.
4. Model preperation using OLS & Linear Regression.
5. Regularization Ridge & Lasso Regression Model.
6. Residual Analysis.
7. Model Evaluation & Assessment.
8. Prediction.
9. Final Conclusion & Analysis.

### Conclusions
Both models of Regression, Lasso and Ridge get positive results to predict sales on housing however Ridge regression provides a result over 91% compared to the 84% of Lasso.

R2_Score for Lasso regresion

#### Ridge Regression
* **Optimal Lambda Value:** 0.02
* **R2 Score Train:** 0.9121057720593937
* **R2 Test Score:**  0.8458706906834216
* **RMSE Test:**      0.016779582835609992

#### Lasso Regression
* **Optimal Lambda Value:** 0.001
* **R2 Score Train:**  0.7897117867370121
* **R2 Test Score:**   0.8454236274425115
* **RMSE Test:**       0.028845649695459316

#### Most Significant Variables are:
The variables that affect the SalePrice are listed from the most significant to the most least used in the regression.

* OverallQual 
* TotSizeAboveGrd 
* GrLivArea 
* GarageCars
* TotalBsmtSF
* 1stFlrSF
* FullBath
* YearBuilt
* YearRemodAdd
* TotRmsAbvGrd
