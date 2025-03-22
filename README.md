# Talco-Customer-churn-analysis
# Customer Churn Prediction using Machine Learning

This repository contains a project focused on predicting customer churn for a telecommunications company using machine learning techniques. The goal of this project is to predict whether a customer will churn based on various features like **Tenure**, **Contract type**, **Service usage**, and **Charges**.

## Project Overview

The project uses Python's popular data analysis and machine learning libraries, including **Pandas**, **NumPy**, **Scikit-learn**, **Matplotlib**, and **Seaborn**, to:

1. **Explore and clean the data** (Exploratory Data Analysis).
2. **Build and evaluate predictive models** for churn using **Logistic Regression** and **Random Forest**.
3. **Tune hyperparameters** using **GridSearchCV** for better model performance.
4. **Apply data balancing techniques** like **SMOTE** to handle class imbalance.
5. **Analyze the most important features** influencing customer churn.

## Dataset

The dataset used in this project contains information about customers' demographics, service usage, and account details. Features include:

- **Tenure**: The number of months the customer has been with the company.
- **Contract**: The type of contract the customer has (Month-to-Month, One Year, Two Year).
- **Service Usage**: Whether the customer has services such as PhoneService, InternetService, OnlineSecurity, TechSupport, etc.
- **Charges**: Monthly charges and total charges for the customer.

## What I Have Learned

### **Customer Behavior Analysis**:
By performing **Exploratory Data Analysis (EDA)**, I identified key customer behaviors that influence churn. **Longer tenure**, **long-term contracts**, and **essential services** like **PhoneService** and **InternetService** tend to reduce churn, while **paperless billing** and **higher charges** correlate with higher churn rates.

### **Modeling Techniques**:
I applied **Logistic Regression** and **Random Forest** classifiers to predict churn. I fine-tuned the models through **GridSearchCV**, experimented with different hyperparameters, and applied **cross-validation** to evaluate model performance. **Logistic Regression** excels at detecting churn with high recall, while **Random Forest** offers a balanced approach with higher precision.

### **Feature Importance**:
Using both **Logistic Regression coefficients** and **Random Forest feature importances**, I identified critical features such as **MonthlyCharges**, **TotalCharges**, **Tenure**, and **Contract** that strongly influence churn predictions.

### **Data Balancing**:
To address the class imbalance in churn prediction, I applied **SMOTE (Synthetic Minority Over-sampling Technique)**. This ensured that the model correctly identified churn cases and improved overall performance.

### **Strategic Application**:
By focusing on high-impact features, businesses can target customers with long tenure or high charges for retention efforts. This analysis helps in **data-driven decision-making** to improve customer retention strategies and reduce churn rates.

## Files in this Repository

1. **Customer Churn.csv**: The dataset containing customer information such as tenure, contract type, service usage, and charges.
2. **Talco_Customer_Churn_Analysis.ipynb**: Jupyter notebook for cleaning, analyzing, and visualizing the churn data, as well as building and evaluating machine learning models.
3. **Executive Summary.pdf**: PDF document summarizing the project, key findings, and recommendations for reducing customer churn based on the analysis.


## How to Run the Code

To run the project on your local machine, you need to have Python 3.x installed along with the following libraries:

- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib**
- **Seaborn**
- **imbalanced-learn** (for SMOTE)

You can install the required dependencies using **pip**:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn imbalanced-learn
