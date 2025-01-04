# **Credit Card Fraud Detection**

This repository contains a Jupyter Notebook that demonstrates how to detect fraudulent credit card transactions using machine learning techniques. The dataset used in this project was sourced from Kaggle.

---

## **Overview**

Credit card fraud is a major concern in the financial industry, and detecting fraudulent transactions is crucial for customer security. This project uses machine learning to classify transactions as fraudulent or non-fraudulent based on anonymized transaction data. The model implemented in this notebook is based on **Logistic Regression**.

The dataset includes features derived using Principal Component Analysis (PCA) and a target variable (`Class`), indicating whether a transaction is fraudulent (`1`) or not (`0`).

---

## **Dataset**

- **Source**: [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Features**:
  - `Time`: Seconds elapsed between the transaction and the first transaction in the dataset.
  - `V1` to `V28`: Principal components obtained using PCA (anonymized for privacy).
  - `Amount`: Transaction amount.
  - `Class`: Target variable (1 = Fraudulent, 0 = Non-fraudulent).
- **Rows**: 284,807 transactions.

---

## **Project Workflow**

1. **Data Loading**:
   - The dataset (`creditcard.csv`) is loaded into a Pandas DataFrame.
2. **Exploratory Data Analysis (EDA)**:
   - Summary statistics and visualizations are used to understand the dataset structure.
3. **Data Preprocessing**:
   - Features are scaled where necessary.
   - The dataset is split into training and testing sets using `train_test_split`.
4. **Model Training**:
   - Logistic Regression is used as the classification model.
5. **Model Evaluation**:
   - Accuracy score is calculated to evaluate the model's performance.

---

## **Dependencies**

To run this project, you need the following Python libraries:

- numpy
- pandas
- scikit-learn

You can install these dependencies using pip:

```bash
pip install numpy pandas scikit-learn
```

---

## **How to Run**

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/CreditCardFraudDetection.git
   cd CreditCardFraudDetection
   ```

2. Ensure that the dataset file (`creditcard.csv`) is in the same directory as the notebook.

3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook CreditCard-Fraud-Detection.ipynb
   ```

4. Run all cells in the notebook to execute the code.

---

## **Results**

The Logistic Regression model provides an accuracy score that indicates its performance in detecting fraudulent transactions. Further improvements can be made by exploring other machine learning models or techniques like oversampling, undersampling, or SMOTE to handle class imbalance.

---

## **Acknowledgments**

- The dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).
- Special thanks to Université Libre de Bruxelles (ULB) for making this dataset available.

---
