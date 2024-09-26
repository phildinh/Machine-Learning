# Employee Clustering Using Unsupervised Learning

## Project Overview
This project applies unsupervised learning techniques to segment employees based on various features such as age, gender, job level, monthly income, and more. The primary goal is to identify distinct groups or clusters within the employee data to understand different employee demographics and behaviors better. The project is organized into several key sections, each outlined below.

## Data Description
The dataset, `employee_data.csv`, consists of demographic and professional details of employees. It includes the following attributes:
- `EmployeeID`: Identification number for employees
- `Age`: Age of the employees
- `Gender`: Gender of the employees
- `DistanceFromHome`: Distance from work to home
- `JobLevel`: Level of job
- `Department`: Department of the employees
- `MonthlyIncome`: Income per month
- `PerformanceRating`: Performance rating
- `JobSatisfaction`: Job satisfaction rating
- `Attrition`: Whether the employee left the company

## Sections of the Project

### 1. Data Preparation & Exploratory Data Analysis (EDA)
- **Data Loading**: Load the data from `employee_data.csv`.
- **Data Cleaning**: Includes converting categorical data into numeric formats using encoding techniques, handling missing values, and removing unnecessary columns.
- **Exploratory Data Analysis**: Provides insights into the dataset by comparing various features against the attrition rate.

### 2. K-Means Clustering
- **Standardizing Data**: Normalize the features to ensure that the distance measure reflects true discrepancies between observations.
- **Model Building**: Fit K-Means clustering models for a range of cluster counts (2 to 15) to determine the optimal number of clusters via the elbow method and silhouette scores.

### 3. PCA for Visualization
- **Dimensionality Reduction**: Apply PCA to reduce features to two principal components for a visual overview of the data distribution and clusters.
- **Visualization**: Visualize the data points in a two-dimensional space with cluster assignments from K-Means to analyze the clustering pattern.

### 4. Second Round of K-Means Clustering
- **Data Refinement**: Exclude potentially less informative features like `Department` to focus on individual attributes.
- **Re-clustering**: Perform K-Means clustering again on this refined dataset to see if the segmentation improves without department data.

### 5. Additional EDA on Clusters
- **Deep Dive into Clusters**: Analyze clusters to understand the demographic and professional characteristics that define each cluster.
- **Attrition Analysis**: Study the attrition rates within each cluster to identify trends and potential risk factors associated with employee turnover.

## Technologies Used
- Python: Main programming language
- Pandas & NumPy: Data manipulation
- Matplotlib & Seaborn: Data visualization
- Scikit-Learn: Implementation of K-Means clustering and PCA

## How to Run the Project
Ensure you have Python installed and the necessary packages added. You can install the requirements via pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
