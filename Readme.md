# README.md

---

## Credit Card Fraud Detection

This repository contains a Jupyter notebook that demonstrates how to detect fraudulent transactions in a credit card dataset using logistic regression.

### Overview

The dataset consists of various credit card transactions, among which a fraction are fraudulent. The primary challenge here is that the dataset is highly unbalanced, meaning there are many more legitimate transactions than fraudulent ones.

### Notebook Contents

1. **Importing Dependencies**:  
    The necessary Python libraries like pandas, numpy, and scikit-learn are imported.

2. **Loading the Dataset**:  
    The dataset named 'creditcard.csv' is loaded into a pandas dataframe.

3. **Initial Data Exploration**:
    - Display the first 5 rows of the dataset.
    - Get information about the dataset like number of entries, column data types, etc.
    - Display the distribution of legitimate vs fraudulent transactions.

4. **Data Analysis**:  
    Separation of the data into legitimate and fraudulent transactions. Statistical measures of the 'Amount' column for both types of transactions are compared.

5. **Under-Sampling**:  
    To tackle the imbalance in the dataset, an under-sampling technique is employed. A sample dataset containing a similar distribution of legitimate and fraudulent transactions is created.

6. **Data Preparation for Model Training**:
    - Split the data into features (`X`) and the target variable (`Y`).
    - Further split the data into training and testing sets.

7. **Model Training**:
    Logistic Regression model from scikit-learn is employed for the training process.

8. **Model Evaluation**:  
    The trained model's performance is evaluated based on its accuracy on the training and testing datasets.

9. **Note**:  
    If there's a significant difference in accuracy between the training and testing data, it indicates that our model might be overfitting or underfitting.

### How to Run

1. Ensure you have the necessary libraries installed. You can install them using pip:

    ``
    pip install pandas numpy scikit-learn
    ``

2. Clone this repository:

    ``
    git clone <repository-url>
    ``

3. Navigate to the directory containing the notebook and run:

    ``
    jupyter notebook
    ``

4. Open the notebook in the Jupyter dashboard and run the cells.

### Dataset

Link: <https://www.kaggle.com/mlg-ulb/creditcardfraud>

The 'creditcard.csv' dataset used in this notebook contains various features related to credit card transactions and a target column named 'Class', where:

- `0` indicates a Legitimate Transaction
- `1` indicates a Fraudulent Transaction
