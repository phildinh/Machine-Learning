# Car Price Prediction Project

## Overview
This project leverages machine learning to predict the selling prices of cars based on various descriptive attributes such as the car's age, mileage, fuel type, and more. The goal is to assist car dealerships and individual sellers in setting competitive and fair prices for used cars.

## Dataset Description
The dataset employed in this project comprises several features pertinent to each car:

- `Car_Name`: Name of the car
- `Year`: Year of manufacture
- `Selling_Price`: Price at which the car is sold (target variable)
- `Present_Price`: Current ex-showroom price of the car
- `Kms_Driven`: Total kilometers driven by the car
- `Fuel_Type`: Type of fuel the car uses (e.g., Petrol, Diesel)
- `Seller_Type`: Type of seller (Dealer or Individual)
- `Transmission`: Type of transmission (Manual or Automatic)
- `Owner`: Number of previous owners

The dataset includes 301 entries, providing a solid basis for the regression model's training and validation.

## Methodology
The project involves the following key stages:

### Data Preprocessing
Initial data cleaning and preprocessing involve handling missing values, encoding categorical variables, and normalizing data as required.

### Feature Selection
Exploratory data analysis helps in selecting significant features that influence the car's selling price most strongly.

### Model Development
A linear regression model is trained using the selected features. The influence of each feature on the selling price is quantified through the model's coefficients.

### Model Evaluation
The model's performance is evaluated using metrics like R-squared, computed on both training and testing data to assess accuracy and generalizability.

### Visualization
Visualization of actual vs. predicted prices helps in visually assessing the model's effectiveness.

## How to Use
To use the model for predicting car prices, follow these steps:

1. **Prepare your data**: Ensure your input data includes the same features as the training dataset and undergoes identical preprocessing steps.
2. **Load the model**: Use the provided serialized model file to load the trained model.
3. **Make predictions**: Use the model's `predict()` method to estimate car prices based on your data.

### Example Usage
```python
import pandas as pd
from sklearn.linear_model import LinearRegression

# Load the trained model (replace 'path_to_trained_model.pkl' with your model's file path)
model = LinearRegression()
model.load('path_to_trained_model.pkl')

# Prepare new data (ensure it's preprocessed as per the training dataset)
new_data = {
    'Year': 2020,
    'Present_Price': 10,
    'Kms_Driven': 25000,
    'Fuel_Type': 'Petrol',
    'Seller_Type': 'Dealer',
    'Transmission': 'Manual',
    'Owner': 0
}
new_data_df = pd.DataFrame([new_data])

# Predict the selling price
predicted_price = model.predict(new_data_df)
print(f"Predicted Selling Price: {predicted_price[0]}")
```


