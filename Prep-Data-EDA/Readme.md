# Customer Subscription Cancellation Prediction

## Overview
This project utilizes a supervised learning approach to predict customer subscription cancellations based on three months of data from Maven Music's customer base. The data includes customer demographics, subscription details, and listening histories. The primary objective is to identify customers who are most likely to cancel their subscriptions and understand the underlying patterns that contribute to this behavior.

## Data Description
The dataset includes three primary files:
- `maven_music_customers.csv`: Contains customer demographic and subscription information.
- `maven_music_listening_history.xlsx`: Includes detailed logs of listening sessions.
- This dataset consists of three sheets: main listening data, audio metadata, and session logs.

## Data Preparation and Cleaning
Data preparation and cleaning are crucial steps in ensuring the quality of the model's predictions. Here are the key tasks performed:

### 1. Data Loading
- Loaded customer data and listening history from CSV and Excel files respectively.
- Excel data required handling multiple sheets which provided session and audio metadata.

### 2. Data Cleaning
- **Type Conversion**: Converted columns to appropriate data types (e.g., dates and numeric formats).
- **Missing Data Handling**: Filled missing values intelligently based on the distribution and relationship of other variables in the dataset. For instance, missing subscription plans were inferred from the subscription rates.
- **Outlier Correction**: Identified and corrected outliers in subscription rates, ensuring data consistency.

### 3. Feature Engineering
- Introduced new features such as `Cancelled` to indicate whether a customer has canceled the subscription.
- Extracted clean email addresses by removing prefixes.
- Derived time-to-cancellation features to capture the duration between subscription start and cancellation dates.

## Exploratory Data Analysis (EDA)
EDA was performed to understand the factors influencing customer behavior and subscription cancellations:
- **Subscription Duration Analysis**: Calculated the average time before cancellation.
- **Discount Impact**: Examined how discounts affect the cancellation rates, finding that customers with discounts are more likely to cancel.
- **Listening Preferences**: Analyzed listening histories to deduce the most popular genres and the relation between genre preferences and subscription cancellations.

### Visualizations
- Created visual representations to better understand customer behaviors and trends. This includes bar charts comparing cancellation rates among different customer groups and plotting listening habits.


