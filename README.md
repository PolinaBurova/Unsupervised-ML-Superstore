# Unsupervised-ML-Superstore

### Customer Segmentation Analysis

This project segments 2,197 customers into distinct groups based on their purchasing behaviors and demographic characteristics using clustering algorithms. The analysis reveals different customer profiles, enabling more targeted marketing strategies, better customer understanding, and improved business decisions.

## Project Structure

- `data/`: Contains the dataset files.
- `notebooks/`: Contains the Jupyter notebook.

### Approach

The analysis involved exploring and cleaning the dataset, followed by feature engineering and preprocessing to prepare the data. Various clustering techniques, including K-Means, Hierchical Clustering and DBSCAN, were then applied to segment customers based on their purchasing behavior and demographics.

### Model Selection

K-Means, chosen for its simplicity and effectiveness, was identified as the best-performing model with the highest silhouette score of 0.23, optimally segmenting the data into two clusters.

![KMeans](https://github.com/PolinaBurova/Unsupervised-ML-Superstore/blob/main/notebooks/KMeans.png)


### Key Results

We then proceeded with the analysis to understand the characteristics of the clusters formed. The process includes fitting the K-Means algorithm, assigning cluster labels, and calculating cluster centers for all features.

**Clustering Process:**

* **Algorithm Used:** K-Means Clustering
* **Number of Clusters:** 2
* **Silhouette Score:** 0.23

![KMeans](https://github.com/PolinaBurova/Unsupervised-ML-Superstore/blob/main/notebooks/clusters.png)

The clustering analysis identified two main customer segments:

* **Cluster 0:** 833 customers (38%)

This cluster generally consists of older individuals who exhibit higher overall spending across various purchasing channels, with a particular focus on products like wine and meat. They tend to have a higher education level, are more likely to be divorced, and often have teenagers at home.

* **Cluster 1:** 1364 customers (62%)

This cluster is generally composed of younger individuals with more focused spending patterns, particularly on deals and specific product categories such as fish, fruits, and sweets. They also have a higher rate of web visits per month, but less purchases. They are more likely to be single and/or married, and have young children at home.

### Ways to further improve the model:

The low silhouette score (0.23) indicates that while there is some structure in the data, the clusters are not highly distinct. This can be attributed to several factors:

**Overlap in Feature Space:** The features used may have significant overlap between clusters, making it hard to distinguish them clearly.

**Intrinsic Data Variability:** The inherent variability in customer behavior and demographics can contribute to less clear-cut clusters.

**Small Dataset Size:** With only around 2,200 rows, the dataset may not provide enough data points to form well-separated clusters. A larger dataset might reveal more distinct groupings.

Despite the low silhouette score, the clustering analysis provides valuable insights into customer segmentation, helping to identify distinct groups based on spending patterns and demographics. This can be useful for targeted marketing strategies and personalized customer engagement.







