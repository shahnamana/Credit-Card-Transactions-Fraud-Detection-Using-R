Certainly! I'll create a README file based on the content of the final report you've provided. Here's a comprehensive README for the GitHub repository:

# Credit Card Transactions Fraud Detection Using R

## Project Overview

This project explores credit card transaction data to detect fraudulent activities using Business Intelligence (BI) models and machine learning techniques implemented in R. We analyze various features of credit card transactions to identify patterns associated with fraud, helping financial institutions and cardholders prevent and mitigate fraud risks.

## Table of Contents

- [Introduction](#introduction)
- [Project Motivation](#project-motivation)
- [Data Description](#data-description)
- [Methodology](#methodology)
- [Key Findings](#key-findings)
- [Machine Learning Models](#machine-learning-models)
- [Repository Structure](#repository-structure)
- [Installation and Usage](#installation-and-usage)
- [Contributors](#contributors)
- [License](#license)

## Introduction

This project was conducted as part of the MIS 6356.006 - Business Analytics with R course in Fall 2022, guided by Professor Zhe Zhang. Our team explored a credit card transactions dataset to derive various BI-based conclusions and findings related to fraud detection.

## Project Motivation

The increasing popularity of online payments and e-commerce has led to a significant rise in credit card fraud. Detecting fraudulent activities is challenging due to the frequent changes in normal and fraudulent behavior profiles and the highly skewed nature of credit card fraud datasets. This project aims to address these challenges and provide insights into fraud detection techniques.

## Data Description

We used a simulated dataset from Kaggle titled "Credit Card Transactions Fraud Detection Dataset." The dataset contains legitimate and fraudulent credit card transactions from 2019 to 2020, including:

- Transactions of 1000 customers and 800 merchants
- 23 columns of data (e.g., transaction date, customer name, merchant name, amount, location)
- Both fraudulent and non-fraudulent transactions

Data source: [Kaggle - Credit Card Transactions Fraud Detection Dataset](https://www.kaggle.com/datasets/kartik2112/frauddetection?select=fraudTrain.csv)

## Methodology

1. Data preprocessing and exploratory data analysis
2. Visualization of fraud patterns across merchant categories and transaction amounts
3. Analysis of customer age in relation to fraud likelihood
4. Implementation of machine learning models:
   - Logistic Regression
   - Decision Tree

## Key Findings

- Merchant categories most prone to fraud:
  - shopping_net and grocery_pos have the highest number of fraudulent transactions
  - shopping_net and shopping_pos involve larger amounts in fraudulent transactions
- No significant evidence that older customers are more likely to be victims of credit card fraud
- Age group 45-60 years showed a slightly higher likelihood of being fraud victims

## Machine Learning Models

### Logistic Regression

We implemented logistic regression to calculate the probability of a fraudulent transaction. However, the model's performance was not optimal due to the need for specifying a cut-off value for predictions.

### Decision Tree

The decision tree model proved to be more effective for this dataset:
- Achieved a 99.3% accuracy rate
- Confusion matrix showed high precision in classifying both fraudulent and non-fraudulent transactions

## Repository Structure

```
├── data/
│   ├── fraudTrain.csv
│   └── fraudTest.csv
│   ├── Online_retail.csv
├── R/
│   ├── BUAN 6356 Group 10 Project.R
│   ├── ML_code.R
├── docs/
│   └── BI.005.10.proposal.Credit Card Transactions Fraud Detection.docx
│   └── Group-10-Final-Report.pdf
├── README.md
└── requirements.R
```

## Installation and Usage

1. Clone the repository:
   ```
   git clone https://github.com/shahnamana/Credit-Card-Transactions-Fraud-Detection-Using-R.git
   ```

2. Navigate to the project directory:
   ```
   cd Credit-Card-Transactions-Fraud-Detection-Using-R
   ```

3. Install required R packages:
   ```R
   source("requirements.R")
   ```

4. Run the R scripts in the `R/` directory to reproduce the analysis.

## Contributors

- Duc Hoang
- Khushi Shah
- Naman Atul Shah
- Rohit Kumar
- Tanay Parag Shah

Guided by Professor Zhe Zhang

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

For more detailed information about the project methodology and findings, please refer to the `Group-10-Final-Report.pdf` file in the `docs/` directory.
