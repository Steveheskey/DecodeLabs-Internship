# DecodeLabs Project 1 — Advanced EDA & Feature Engineering

## Project Overview

This project was completed as part of the DecodeLabs Data Science Internship Programme.

The objective of the project is to transform a raw customer dataset into a clean, structured and machine-learning-ready dataset through exploratory data analysis, statistical imputation, outlier treatment and feature engineering.

## Project Objectives

The project focuses on:

- Performing exploratory data analysis (EDA)
- Identifying and handling missing values
- Detecting and neutralizing outliers using the Interquartile Range (IQR) method
- Engineering at least three new predictive features
- Validating the final cleaned dataset
- Saving the processed dataset for future machine-learning applications

## Dataset

The dataset contains customer-level information including:

- Customer ID
- Age
- Annual Income
- Tenure
- Monthly Spend
- Orders in the Last 12 Months
- Satisfaction Score
- Complaints
- Support Calls
- Discount Percentage
- Region
- Customer Segment
- Payment Method

The dataset was prepared for this project to provide realistic data-cleaning and feature-engineering challenges, including missing values, duplicate records and extreme observations.

## Data Cleaning Process

### 1. Exploratory Data Analysis

Initial analysis was performed to understand:

- Dataset dimensions
- Data types
- Missing values
- Descriptive statistics
- Duplicate records
- Variable distributions
- Skewness

### 2. Missing Value Treatment

Missing values were identified and treated using statistical imputation.

Mean imputation was applied to relatively symmetrical variables, while median imputation was used for highly skewed variables where extreme observations could distort the mean.

### 3. Duplicate Records

Duplicate records were identified during the initial data-quality assessment and removed before further statistical processing.

### 4. Outlier Detection

The Interquartile Range (IQR) method was used to identify extreme observations.

The IQR was calculated as:

IQR = Q3 - Q1

Lower Bound = Q1 - 1.5 × IQR

Upper Bound = Q3 + 1.5 × IQR

### 5. Outlier Treatment

Instead of deleting observations, identified extreme values were capped at the calculated IQR boundaries.

This preserved the observations while reducing the influence of extreme values on statistical analysis.

## Feature Engineering

Three new features were created from existing variables:

### Monthly Income

Estimated monthly income was calculated from annual income.

### Spend-to-Income Ratio(Spending Ratio)

This measures monthly spending relative to estimated monthly income.

### Orders per Tenure Month

This measures purchasing frequency relative to the customer's tenure.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- VS Code
- Git

- ## Conclusion

The project demonstrates a complete data-preparation workflow, transforming raw customer data into a cleaner and more structured dataset suitable for subsequent machine-learning analysis.

The workflow covers exploratory data analysis, missing-value treatment, duplicate removal, IQR-based outlier treatment and feature engineering.

## Project Structure

```text
Decode Labs/
│
├── data/
│   ├── raw dataset
│   └── final cleaned dataset
│
├── notebooks/
│   └── Decode_Labs Prj 1.ipynb
│
├── src/
│
├── .gitignore
├── README.md
└── requirements.txt

