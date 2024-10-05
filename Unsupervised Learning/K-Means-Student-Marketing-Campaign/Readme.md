# Customer Segmentation Analysis 🎯

## Tools Used
- **Python** 🐍: For data manipulation, clustering, and analysis.
- **Excel** 📊: For initial data review and verification of columns and rows.
- **Pandas** & **NumPy**: For data handling.
- **Matplotlib** & **Seaborn**: For data visualization.
- **Scikit-learn**: For implementing machine learning algorithms.
- **Jupyter Notebook**: For coding and visualizations.

## Introduction 📌
This project focuses on clustering techniques to segment customers based on their entertainment preferences, helping tailor marketing strategies effectively. Understanding these preferences allows for optimized marketing campaigns that are more aligned with the target audience's behavior.

## Aim of the Project 🎯
The primary aim of this project is to enhance marketing strategies by identifying distinct customer groups through their entertainment consumption patterns. This involves:
- **Segmenting customers** to understand diverse preferences.
- **Tailoring marketing messages** based on segment-specific behaviors.
- **Optimizing marketing resources** by focusing on effective channels.
- **Increasing campaign effectiveness**, leading to higher engagement and customer loyalty.

## Methodology 🔍
1. **Data Collection**
   - Data includes weekly hours spent on reading books, watching movies, TV shows, and playing video games.
   
2. **Data Preprocessing**
   - Creation of a pivot table to structure data appropriately.
   - Filling missing values and removing duplicates.
   - Verification and type-checking of data fields.

3. **Data Analysis**
   - Conducted EDA to explore data characteristics.
   - Normalized data using `StandardScaler`.

4. **Clustering**
   - Applied K-means clustering to identify customer segments.
   - Used the Elbow Method and Silhouette Score to find the optimal cluster count.
   - Analyzed cluster characteristics to define each segment.

5. **Results Implementation**
   - Labeled each customer profile with their respective cluster.
   - Developed targeted marketing strategies based on cluster analysis.

## Requirements 📋
- Python 3.8 or higher
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`
- Data: Ensure the dataset includes customer names and their respective hours spent on different entertainment activities.

## Results 📈
Identified 3 distinct segments with unique entertainment preferences which were used to formulate targeted marketing strategies:
1. **Segment 1**: Prefers TV shows.
2. **Segment 2**: Favors books and movies.
3. **Segment 3**: Enjoys video games and books.

## Conclusion 🚀
The application of clustering techniques has provided significant insights into customer preferences, enabling the development of more refined and targeted marketing strategies. Further analysis will include demographic variables for deeper segmentation.


