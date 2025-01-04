# **Credit Card Fraud Detection**

This repository contains a Jupyter Notebook for detecting fraudulent credit card transactions using a logistic regression model. The dataset used for this project was obtained from Kaggle.

---

## **Overview**

Credit card fraud is a significant issue in the financial sector, and detecting fraudulent transactions is critical for ensuring customer security. This project demonstrates how to use machine learning techniques to classify transactions as fraudulent or non-fraudulent.

The dataset includes anonymized transaction features (`V1`, `V2`, ..., `V28`), the transaction amount (`Amount`), and the time of the transaction (`Time`). The target variable (`Class`) indicates whether a transaction is fraudulent (1) or not (0).

---

## **Dataset**

- **Source**: [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Features**:
  - `Time`: Seconds elapsed between the transaction and the first transaction in the dataset.
  - `V1` to `V28`: Principal components obtained using PCA (anonymized for privacy).
  - `Amount`: Transaction amount.
  - `Class`: Target variable (0 = Non-fraudulent, 1 = Fraudulent).

---

## **Project Workflow**

1. **Data Loading**: The dataset is loaded into a Pandas DataFrame.
2. **Exploratory Data Analysis (EDA)**: A brief overview of the dataset structure.
3. **Model Training**:
   - Logistic Regression is used as the classification model.
   - The dataset is split into training and testing sets using `train_test_split`.
4. **Model Evaluation**:
   - The accuracy of the model is calculated using `accuracy_score`.

---

## **Dependencies**

To run this project, you need the following Python libraries:

- pandas
- numpy
- scikit-learn

You can install these dependencies using pip:

```bash
pip install pandas numpy scikit-learn
```

---

## **How to Run**

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/MyJupyterNotebook.git
   cd MyJupyterNotebook
   ```

2. Ensure that the dataset (`creditcard.csv`) is in the same directory as the notebook.

3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook main_001.ipynb
   ```

4. Run all cells in the notebook to execute the code.

---

## **Results**

The logistic regression model provides an accuracy score that indicates its performance in detecting fraudulent transactions. Further improvements can be made by exploring other machine learning models or techniques.

---

## **Acknowledgments**

- The dataset was provided by [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).
- Special thanks to Université Libre de Bruxelles (ULB) for making this dataset available.

---
