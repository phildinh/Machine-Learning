# Enhanced Customer Segmentation in Wholesale Distribution 📊

## Project Overview
This project leverages advanced clustering techniques to refine customer segmentation for a wholesale distributor by identifying outliers and grouping similar entities effectively. Using a combination of DBSCAN for outlier detection and KMeans for precise clustering, this approach optimizes marketing strategies and resource allocation based on customer behaviors and purchasing patterns.

## Data Preparation
The dataset `wholesale_clients.csv` includes purchasing details of clients categorized by product categories such as Fresh, Milk, Grocery, Frozen, Detergents_Paper, and Delicassen. Initial steps include:
- Removal of non-essential features (`Channel`, `Region`) to focus the analysis on product spending.
- Standardization of data to ensure uniformity for advanced analytical techniques.

## Methodology

### 1. **Outlier Detection with DBSCAN** 🔍
- Utilized the DBSCAN algorithm to identify and exclude outliers in the dataset, enhancing the quality of subsequent clustering.
- Parameters like `eps` and `min_samples` were fine-tuned to optimize the clustering outcome, guided by silhouette scores.

### 2. **Clustering with KMeans** 📈
- Applied the KMeans clustering algorithm on the cleaned and scaled data to group clients into meaningful clusters based on their purchasing behavior.
- The number of clusters was determined by analyzing the inertia and silhouette scores, selecting the optimal balance for detailed yet distinct grouping.

### 3. **Visualization with PCA** 🌐
- Performed Principal Component Analysis (PCA) to reduce dimensionality and visualize the data in a two-dimensional space, aiding in understanding the spread and grouping of clusters.

## Results
- Identification of distinct customer segments that exhibit unique purchasing behaviors, which can be targeted with tailored marketing strategies.
- Enhanced understanding of the data structure and distribution through PCA, highlighting the relationships and differences between various customer groups.

## Tools and Libraries Used
- **Pandas**: For data manipulation and analysis.
- **Scikit-learn**: For implementing standard scaling, DBSCAN, KMeans, and PCA.
- **Matplotlib & Seaborn**: For plotting and visualizing data.

## Conclusion
This project demonstrates the effectiveness of combining multiple clustering techniques to improve customer segmentation. The insights derived from this analysis provide a foundation for developing targeted marketing strategies that cater to the specific needs and behaviors of different customer segments in the wholesale distribution sector.

## Repository Contents
- Data preparation and cleaning notebooks.
- DBSCAN tuning and application scripts.
- KMeans clustering implementation and results analysis.
- PCA visualization scripts.
- Documentation and presentation materials.
