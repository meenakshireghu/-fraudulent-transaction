# Fraud Detection Using Machine Learning
This project analyzes and detects fraudulent transactions in a dataset using machine learning techniques. The primary goal is to classify transactions as either fraudulent or non-fraudulent. The analysis involves data exploration, visualization, and modeling using Logistic Regression.

## Dataset Overview

The dataset used in this project contains details of various financial transactions, including:
- **Columns**:
  - `step`: Time step of the transaction (dropped in preprocessing).
  - `type`: Type of transaction (e.g., CASH_OUT, TRANSFER).
  - `amount`: Amount of the transaction.
  - `oldbalanceOrg` and `newbalanceOrig`: Original and new balances of the origin account.
  - `oldbalanceDest` and `newbalanceDest`: Original and new balances of the destination account.
  - `isFraud`: Indicates whether the transaction is fraudulent (1) or not (0).
  - `isFlaggedFraud`: Indicates whether the transaction was flagged as fraud (dropped in preprocessing).
  # Project Workflow

1. **Data Preprocessing**:
   - Removed unnecessary columns: `step`, `nameOrig`, `nameDest`, and `isFlaggedFraud`.
   - Checked for null values and explored dataset structure.
   - Encoded categorical variables using one-hot encoding.
   - Standardized numerical features using `StandardScaler`.

2. **Exploratory Data Analysis (EDA)**:
   - Analyzed the proportion of fraudulent and non-fraudulent transactions using a pie chart.
   - Visualized the distribution of fraud types using a bar chart.
   - Generated a correlation heatmap for numerical features.

3. **Model Building**:
   - **Logistic Regression**:
     - Trained a logistic regression model.
     - Evaluated model performance using accuracy, confusion matrix, classification report, and cross-validation.

4. **Model Evaluation**:
   - Evaluated the performance of the Logistic Regression model.
