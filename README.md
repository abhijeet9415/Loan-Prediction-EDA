# Loan Approval Data Prediction

## Description
This project predicts the loan approval status of applicants based on various features using machine learning. The notebook explores data preprocessing, feature engineering, and model training to build a prediction model. The dataset includes information on applicants like income, education, loan amount, and credit history.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Data](#data)
- [Models and Methods](#models-and-methods)
- [Results](#results)

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/loan-approval-prediction.git
    ```

2. **Navigate to the project folder**:
    ```bash
    cd loan-approval-prediction
    ```

3. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Run the Jupyter Notebook**:
    ```bash
    jupyter notebook eda-of-financial-data.ipynb
    ```

## Usage

1. **Open the Jupyter Notebook**: You can explore the notebook `eda-of-financial-data.ipynb` to review the data analysis and machine learning steps.
   
2. **Model Training and Testing**: The notebook includes code to preprocess the data, train models, and evaluate performance.

3. **Prediction**: After training, you can make predictions on new data by running the model.

## Features
- **Data Preprocessing**: Handled missing values by using mode and mean for categorical and numerical variables, respectively.
- **Exploratory Data Analysis (EDA)**: Performed analysis of various features and their relationship with the target variable.
- **Loan Approval Prediction**: Used Logistic Regression to build the prediction model.
- **Model Evaluation**: Evaluated model accuracy on both training and test datasets.

## Data

The dataset used for the project includes the following columns:

- **Loan_ID**: Unique identifier for each loan
- **Gender**: Gender of the applicant
- **Married**: Marital status of the applicant
- **Dependents**: Number of dependents
- **Education**: Education level of the applicant
- **ApplicantIncome**: Income of the applicant
- **CoapplicantIncome**: Income of the co-applicant
- **LoanAmount**: The amount of loan
- **Loan_Amount_Term**: Term of the loan in months
- **Credit_History**: History of credit repayment (1 = Yes, 0 = No)
- **Loan_Status**: Whether the loan was approved (Y) or not (N)

## Models and Methods

- **Logistic Regression**: This model was used to predict whether the loan will be approved.
  - **Accuracy**: 77.27% on the test dataset.
  - **Cross-validation**: Achieved an 80.95% accuracy using cross-validation (5-fold).
  
- **Data Cleaning and Feature Engineering**:
  - Imputation of missing values in key features like `LoanAmount` and `Credit_History`.
  - Log transformation applied to reduce skewness in the `LoanAmount` feature.
  
- **Evaluation Metrics**:
  - **Accuracy**: Measured the percentage of correct predictions.
  - **Cross-Validation Score**: Assessed the generalization ability of the model.

## Results

- Logistic Regression provided an accuracy of 77.27% on the test data.
- Cross-validation increased the model’s performance to 80.95%.
- Some key insights:
  - Applicants with higher income had a higher probability of loan approval.
  - Credit history had a significant impact on loan approval decisions.




