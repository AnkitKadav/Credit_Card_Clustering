Credit Card Customer Segmentation using Clustering

Overview

This project aims to segment credit card holders into distinct groups based on their spending behavior and financial habits. By leveraging unsupervised learning techniques, specifically K-means clustering, we analyzed a dataset of 9,000 credit card holders to extract insights useful for targeted marketing and customer management.

Table of Contents

Introduction

Dataset

Data Preprocessing

Clustering with K-means

Dimensionality Reduction with PCA

Business Insights

Conclusion

Next Steps

How to Run the Project

Code Explanation

Contributors

License

Introduction

Objective: The goal of this project is to group customers into clusters based on their spending patterns and financial behavior. These clusters will help businesses create more personalized marketing strategies and improve customer satisfaction.

Dataset

The dataset includes 18 behavioral features of 9,000 credit card holders over six months.

Features include balance, purchase frequency, credit limit, and payments.

Data Preprocessing

Missing Values: Missing values in features such as MINIMUM_PAYMENTS were imputed using the median.

Dropped Columns: Unnecessary columns were removed to reduce noise and focus on key financial behaviors.

Correlation Analysis: Feature correlations were analyzed to understand relationships between variables like PURCHASES, CREDIT_LIMIT, and BALANCE.

Clustering with K-means

K-means Algorithm: Applied K-means clustering and determined that 4 clusters were optimal using the elbow plot and silhouette score.

Cluster Characteristics:

Cluster 1: Customers with low credit limits but frequent purchases.

Cluster 2: Customers with high balances and large one-off purchases.

Cluster 3: Customers who frequently take cash advances.

Cluster 4: Customers with high credit limits but low purchase frequency.

Dimensionality Reduction with PCA

Why PCA? PCA was used to reduce data dimensionality while preserving important information, making clusters clearer.

Results: PCA improved clustering results by simplifying customer behavior into key components.

Business Insights

Targeted Marketing: Different clusters allow businesses to design personalized offers.

Cluster 2 might respond well to high-value promotions.

Cluster 1 could benefit from frequent-purchase loyalty programs.

Credit Risk Management: Customers in Cluster 3, who frequently take cash advances, might require closer monitoring.

Product Recommendations: Businesses can offer tailored credit card products, such as higher limits or installment-based offers, based on cluster characteristics.

Conclusion

This project successfully segmented credit card customers into four distinct groups, each with unique spending behaviors. The insights gained can help businesses develop targeted marketing strategies, improve customer satisfaction, and optimize credit risk management. PCA further refined clustering results, making insights clearer and more actionable.

Next Steps

Further Analysis: Explore additional clustering techniques like hierarchical clustering for comparison.

Implementation: Integrate findings into business marketing and risk management strategies.

How to Run the Project

Clone the repository:

git clone https://github.com/your-repo-name.git

Navigate to the project directory:

cd your-repo-name

Install required dependencies:

pip install -r requirements.txt

Run the Jupyter Notebook to execute the analysis:

jupyter notebook clustering_analysis.ipynb

Code Explanation

data_preprocessing.py

This script handles missing values, removes unnecessary columns, and performs correlation analysis to prepare the dataset for clustering.

kmeans_clustering.py

This script applies the K-means algorithm, determines the optimal number of clusters using the elbow method and silhouette score, and visualizes the clustered data.

pca_analysis.py

This script implements Principal Component Analysis (PCA) to reduce the dataset’s dimensionality, enhancing the clarity of clustering results.

business_insights.py

This script interprets the clusters and provides actionable insights for targeted marketing and credit risk management.

Contributors

Disha Raskar

Achal Jajoo

Ankit Kadav

License

This project is licensed under the MIT License.
