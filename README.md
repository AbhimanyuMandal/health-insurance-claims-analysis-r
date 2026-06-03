# 🏥 Health Insurance Claims Analysis using R

## 📌 Project Overview

This project performs an end-to-end analysis of health insurance claims data using R, covering data cleaning, feature engineering, exploratory data analysis (EDA), statistical testing, and predictive modeling.

The objective is to identify factors associated with claim approval, fraud risk, settlement outcomes, and operational inefficiencies within the claims process.

The analysis demonstrates practical applications of healthcare analytics, statistical modeling, and business intelligence techniques using a real-world insurance claims dataset.
---

## Dataset

Dataset: Indian Health Insurance Claims Data

Source: Kaggle

https://www.kaggle.com/datasets/apurvpanchal/indian-health-insurance-claims-data

This dataset is a synthetic healthcare insurance claims dataset designed for analytics, fraud detection, and predictive modeling applications.

---

## 🎯 Project Objectives

This analysis aims to answer:

* Which factors influence claim approval?
* How does documentation completeness affect claim outcomes?
* Are high-risk hospitals associated with increased fraud rates?
* What characteristics are associated with claim rejection?
* Can claim approval be predicted using patient, provider, and claim-related variables?

---

## 🛠️ Tools & Technologies

###Programming Language:

* R

###Libraries:

* tidyverse
* dplyr
* ggplot2
* janitor
* skimr
* corrplot
* broom
* scales

###Statistical Methods:

* Descriptive Statistics
* Chi-Square Testing
* Correlation Analysis
* Logistic Regression

---

## 📂 Project Structure

```text
health-insurance-claims-analysis-r/
│
├── README.md
├── requirements.R
│
├── data/
│   ├── raw/
│   └── processed/
|
├── scripts/
│   ├── 01_import_and_clean.R
│   ├── 02_feature_engineering.R
│   ├── 03_eda.R
│   ├── 04_statistical_analysis.R
│   └── 05_export_cleaned_data.R
│
outputs/
├── figures/
│   ├── claim_status_by_document_status.png
│   ├── claim_amount_distribution.png
│   ├── settlement_rate_by_diagnosis.png
│   └── correlation_matrix.png
│
└── tables/
|   ├── fraud_by_accreditation.csv
|   └── logistic_regression_summary.csv
|
└── docs/
```

---

## 🔧 Data Cleaning

The following preprocessing steps were performed:

* Standardized column names using clean_names()
* Removed duplicate observations
* Converted categorical variables into factors
* Checked data structure and missing values
* Generated descriptive summaries using skimr

---

## ⚙️ Feature Engineering

Several analytical variables were created:

| Feature            | Description                            |
| ------------------ | -------------------------------------- |
| approval_flag      | Approved = 1, Rejected = 0             |
| fraud_flag         | Fraud identified = 1                   |
| claim_loss         | Claimed amount − Settled amount        |
| settlement_rate    | Percentage of claim settled            |
| high_risk_provider | Blacklisted provider or risk score ≥70 |
| doc_complete_flag  | Complete documentation indicator       |
| delay_bucket       | Claim submission delay category        |

---

## 📊 Exploratory Data Analysis

The analysis includes:

### Claim Status by Documentation

Evaluates whether document completeness influences approval rates.

### Claim Amount Distribution

Examines claim size patterns across the portfolio.

### Settlement Rate by Diagnosis

Identifies diagnosis categories associated with lower settlements.

### Fraud Risk Assessment

Compares fraud rates and approval rates across hospital accreditation groups.

---

## 📈 Statistical Analysis

### Chi-Square Tests

Used to assess associations between:

* Document status and claim outcome
* Provider blacklist status and claim outcome

### Logistic Regression

A binary logistic regression model was built to estimate the probability of claim approval.

Predictors include:

* Age
* Fraud flag
* Hospital risk score
* Documentation completeness
* Claim submission delay
* Provider blacklist status

---

## 📉 Correlation Analysis

A correlation matrix was generated for all numerical variables to identify potential relationships and multicollinearity.

---

## 🚀 Key Skills Demonstrated

* Data Cleaning
* Feature Engineering
* Exploratory Data Analysis
* Statistical Testing
* Logistic Regression
* Data Visualization
* Reproducible Research
* Healthcare Analytics
* Insurance Analytics

---

## 📚 Reproducibility

Run the project in sequence:


source("requirements.R")
source("scripts/01_import_and_clean.R")
source("scripts/02_feature_engineering.R")
source("scripts/03_eda.R")
source("scripts/04_statistical_analysis.R")
source("scripts/05_export_cleaned_data.R")


---

## 🔮 Future Improvements

* Random Forest Classification
* XGBoost Claim Approval Prediction
* Fraud Detection Models
* Interactive Dashboard using Shiny
* Automated Reporting using Quarto

---

## 👤 Author

**Abhimanyu Mandal**

Biomedical Data Analyst | Bioinformatics Researcher | Data Analyst

Interests:

* Healthcare Analytics
* Cancer Genomics
* Machine Learning
* Statistical Modeling
* Real-World Data Analysis

LinkedIn:
https://www.linkedin.com/in/abhimanyu-mandal/
