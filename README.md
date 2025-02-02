# Clustering Evaluation on Iris Dataset
This project applies and evaluates multiple clustering algorithms on the Iris dataset. It utilizes different preprocessing techniques and clustering methods to analyze the dataset and compare the models' performance using various evaluation metrics.

## Introduction
In this project, we evaluate three popular clustering algorithms:

- KMeans: A centroid-based clustering algorithm.
- DBSCAN: A density-based clustering algorithm.
- Agglomerative Clustering: A hierarchical clustering algorithm.
We apply these clustering algorithms on the Iris dataset using different preprocessing techniques (Standardization, Normalization, and PCA transformation) and evaluate their performance using various clustering evaluation metrics.

## Data Preprocessing
Before applying the clustering algorithms, the dataset is preprocessed in the following ways:

- Standardization: This technique scales the data so that it has a mean of 0 and a standard deviation of 1.
- Normalization: This technique scales the data to a range between 0 and 1 using MinMaxScaler.
- PCA (Principal Component Analysis): This technique reduces the dimensionality of the data to 2 components for easier visualization while preserving the variance.

## Clustering Algorithms
The following clustering algorithms are applied:

- KMeans: KMeans tries to partition the data into k clusters, minimizing the variance within clusters.
- DBSCAN: DBSCAN groups together points that are close to each other, marking points in low-density regions as outliers.
- Agglomerative Clustering: A hierarchical clustering algorithm that builds clusters by iteratively merging smaller clusters.
  
## Parameters for Testing:
- KMeans and Agglomerative Clustering: We test with different values of clusters (k = 1, 3, 5).
- DBSCAN: We apply the algorithm with default parameters (eps=0.5, min_samples=5).
## Evaluation Metrics
The performance of the clustering algorithms is evaluated using the following metrics:

- Silhouette Score: Measures how similar each point is to its own cluster compared to other clusters.
- Davies-Bouldin Score: Measures the average similarity ratio of each cluster with the cluster that is most similar to it. Lower scores are better.
- Calinski-Harabasz Score: Measures the ratio of the sum of between-cluster dispersion to within-cluster dispersion. Higher scores are better.
## Visualization
The results of clustering algorithms are visualized using Principal Component Analysis (PCA) to reduce the dataset to two dimensions. The visualizations help to visually inspect the clusters formed by each algorithm.

### PCA Plots:
The PCA transformation is applied to each clustering result, and a scatter plot is created to visualize the clustering of data points.
![download (25)](https://github.com/user-attachments/assets/143879f8-5440-4dc3-9f82-36b8130e902a)
![Screenshot 2025-02-01 at 10 18 49 PM](https://github.com/user-attachments/assets/ecb46811-133a-4bec-b84b-109cacefb167)

