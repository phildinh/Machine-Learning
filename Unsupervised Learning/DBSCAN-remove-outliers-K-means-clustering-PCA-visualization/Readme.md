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

![image](https://github.com/user-attachments/assets/38557ade-9f82-4c54-b703-35fc7f407dad)

- Cluster 0 (Low Spend Group): Characteristics: This cluster generally shows low spending across all categories, with no particularly strong emphasis on any single product category. Suggested Name: "Minimal Spenders" or "Low Volume Shoppers"
- Cluster 1 (Diverse High Spend Group): Characteristics: This group spends heavily across several categories, particularly on 'Milk', 'Grocery', and 'Detergents_Paper'. They also show significant spending in 'Delicassen'. Suggested Name: "Broad Range High Spenders" or "Versatile Big Spenders"
- Cluster 2 (Selective High Spend Group): Characteristics: Members of this cluster show notably high expenditure specifically in the 'Delicassen' category, with moderate to low spending in other areas. Suggested Name: "Delicatessen Enthusiasts" or "Specialty Goods Shoppers"
- Cluster 3 (Fresh and Frozen Focus Group): Characteristics: This cluster has high spending in 'Fresh' and 'Frozen' categories, indicating a preference for perishable and frozen goods, possibly suggesting a focus on quality or freshness. Suggested Name: "Fresh and Frozen Food Lovers" or "Perishable Goods Preferers"

- Cluster 0: "Basic Buyers"
- Cluster 1: "Super Shoppers"
- Cluster 2: "Gourmet Gurus"
- Cluster 3: "Fresh Favorites"
### 3. **Visualization with PCA** 🌐
- Performed Principal Component Analysis (PCA) to reduce dimensionality and visualize the data in a two-dimensional space, aiding in understanding the spread and grouping of clusters.

![image](https://github.com/user-attachments/assets/d8261886-1074-49e7-81f8-cac01ea92b0c)

- Component 1: Higher spending on non-perishables (Milk, Grocery, Detergents).
- Component 2: Higher spending on perishables (Fresh, Frozen).

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
