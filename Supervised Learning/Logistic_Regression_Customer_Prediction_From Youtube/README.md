# Customer Churn Prediction Using Logistic Regression

## Introduction
This project leverages logistic regression to predict customer churn based on a comprehensive dataset encompassing customer demographics and transactional behavior. The analysis aims to identify key factors contributing to customer attrition, enabling the development of targeted strategies to enhance customer retention.

## Project Structure
- `data/`: Directory containing the dataset used in the analysis.
- `scripts/`: Python scripts for data preprocessing, model building, and evaluation.
- `notebooks/`: Jupyter notebooks with detailed analysis steps and observations.
- `reports/`: Generated analysis reports and insights summary.

## Dataset Overview
The dataset includes 10,000 customer records with the following features:
- **Age**: Age of the customer.
- **Income**: Customer's annual income.
- **Gender**: Customer's gender (Male/Female).
- **Marital_Status**: Marital status (Single/Married).
- **Transaction_Count**: Total number of transactions.
- **Product_Category**: Categories of purchased products (Electronics, Clothing, Food).
- **Engagement_Score**: Customer engagement score.
- **Churn**: Binary indicator of churn (1 = churned, 0 = not churned).

## Data Exploration
The initial exploration focuses on understanding the dataset's structure, identifying missing values, and summarizing statistical properties of the features. Insights from this phase guide the preprocessing and feature engineering steps.

## Data Preprocessing
This step involves:
- Encoding categorical variables to numeric format to ensure compatibility with the logistic regression algorithm.
- Handling missing values, if any.
- Normalizing or standardizing continuous variables to improve model performance.

## Model Development
A logistic regression model is built using the preprocessed data. The process includes:
- Splitting the data into training and testing sets.
- Using the training set to train the logistic regression model.
- Applying the trained model to the test set to evaluate its predictive performance.

## Model Evaluation
The model's performance is evaluated through various metrics:
- **Accuracy**: Overall correctness of the model.
- **Confusion Matrix**: To assess the number of correct and incorrect predictions for each class.
- **Precision, Recall, and F1-Score**: To understand the balance between recall and precision.

## Model Interpretation
The coefficients of the logistic regression model are interpreted to determine the influence of each feature on the likelihood of customer churn. This interpretation helps in understanding how different factors impact customer retention.

## Conclusions and Business Insights
The final section outlines the key findings from the model and suggests actionable strategies based on the insights gained. It includes recommendations on focusing retention efforts on identified key drivers of churn.

## How to Run the Project
Instructions on setting up the environment, installing dependencies, and running the scripts and notebooks for reproducing the analysis results.

## Authors
- Phil Dinh

## Acknowledgments
- Thanks to professor Frederick Nwanganga for guidance

