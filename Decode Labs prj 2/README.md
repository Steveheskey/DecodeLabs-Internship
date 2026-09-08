# DecodeLabs Project 2 — Credit Card Fraud Detection

## 📌 Project Overview

This project focuses on detecting fraudulent credit card transactions using **Machine Learning classification techniques**.

Credit card fraud detection is a highly imbalanced classification problem because fraudulent transactions typically represent only a very small proportion of all transactions. Therefore, the project focuses not only on building predictive models but also on selecting appropriate evaluation metrics for measuring fraud detection performance.

The project was completed as part of the **DecodeLabs Data Science Internship**.

---

## 🎯 Project Objective

The main objective of this project is to develop a machine learning model capable of distinguishing between:

* **Legitimate transactions**
* **Fraudulent transactions**

The project explores the dataset, performs data preprocessing, handles the class imbalance, trains machine learning models, and evaluates their performance using appropriate classification metrics.

---

## 📂 Dataset

The dataset used for this project is the **Credit Card Fraud Detection Dataset** from Kaggle.

**Source:** Kaggle — Credit Card Fraud Detection

Dataset:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

The dataset contains credit card transactions made by European cardholders over two days.

### Dataset Structure

The dataset contains:

* `Time` — Seconds elapsed between each transaction and the first transaction
* `V1` to `V28` — Principal Component Analysis (PCA) transformed features
* `Amount` — Transaction amount
* `Class` — Target variable

### Target Variable

The `Class` column represents whether a transaction is fraudulent:

| Class | Meaning                |
| ----- | ---------------------- |
| 0     | Legitimate transaction |
| 1     | Fraudulent transaction |

---

## 🛠️ Technologies Used

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## 🔍 Project Workflow

The project follows the following machine learning workflow:

### 1. Data Loading

The dataset was imported into Python using Pandas and inspected to understand its structure.

### 2. Exploratory Data Analysis

The dataset was explored to identify:

* Number of transactions
* Number of fraudulent transactions
* Number of legitimate transactions
* Data types
* Missing values
* Duplicate records
* Distribution of transaction amounts
* Distribution of the target variable

### 3. Data Preprocessing

The data was prepared for machine learning by:

* Checking for missing values
* Checking for duplicate records
* Separating features from the target variable
* Scaling relevant numerical variables where necessary
* Splitting the dataset into training and testing sets

### 4. Handling Class Imbalance

Because fraudulent transactions are significantly fewer than legitimate transactions, class imbalance was considered during model development.

Appropriate techniques were explored to prevent the models from simply predicting the majority class.

### 5. Model Development

Machine learning classification algorithms were trained and evaluated to determine which approach performs best at identifying fraudulent transactions.

### 6. Model Evaluation

The models were evaluated using metrics that are appropriate for an imbalanced classification problem, including:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix
* ROC-AUC

Particular attention was given to **Recall**, because failing to identify a fraudulent transaction can be more costly than incorrectly flagging a legitimate transaction.

---

## 📊 Evaluation Metrics

### Accuracy

Measures the proportion of all predictions that were correct.

### Precision

Measures how many transactions predicted as fraudulent were actually fraudulent.

### Recall

Measures how many actual fraudulent transactions were successfully detected.

### F1-Score

Provides a balance between precision and recall.

### ROC-AUC

Measures the model's ability to distinguish between fraudulent and legitimate transactions across different classification thresholds.

---

## 📁 Project Structure

```text
DecodeLabs Project 2/
│
├── Data Set/
│   └── creditcard.csv
│
├── Decode Labs Prj 2.ipynb
│
└── README.md
```

---

## ▶️ How to Run the Project

### 1. Clone or download this repository

Download the project repository to your computer.

### 2. Download the dataset

Download the Credit Card Fraud Detection dataset from Kaggle:

https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

### 3. Add the dataset

Place the downloaded `creditcard.csv` file inside:

```text
Data Set/
```

### 4. Open the notebook

Open:

```text
Decode Labs Prj 2.ipynb
```

using Jupyter Notebook or JupyterLab.

### 5. Run the notebook

Run all cells from beginning to end to reproduce the analysis and model results.

---

## 📌 Key Learning Outcomes

Through this project, I applied machine learning concepts including:

* Exploratory Data Analysis
* Data preprocessing
* Feature and target separation
* Train-test splitting
* Feature scaling
* Imbalanced classification
* Classification algorithms
* Model evaluation
* Confusion matrix interpretation
* Precision and recall analysis
* Fraud detection using Machine Learning

---

## 👤 Author

**Stephen Emesiana**
Data Science Enthusiast 
