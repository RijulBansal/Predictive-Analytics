# Clustering Analysis on UCI Wine Dataset

## Overview

This project performs clustering analysis on the UCI Wine Dataset using three clustering algorithms: K-Means, Hierarchical Clustering, and Mean-Shift Clustering. The dataset is preprocessed, analyzed using multiple clustering techniques, evaluated using various metrics, and visualized using different plots.

## Dataset

The dataset used is the Wine dataset from the UCI Machine Learning Repository. It consists of chemical analysis of wines grown in the same region in Italy but derived from three different cultivars.

## Features:

- 13 numerical attributes related to wine characteristics

- Target variable (wine class) is ignored for unsupervised clustering

  ## Steps in the Analysis

  ## 1. Data Preprocessing
- Standardization using StandardScaler

- Dimensionality reduction using PCA

- Transformation techniques applie

2. Clustering Algorithms Used

- K-Means Clustering (with Elbow Method for optimal K selection)

- Hierarchical Clustering (Agglomerative)

- Mean-Shift Clustering

3. Performance Evaluation Metrics

- Silhouette Score

- Calinski-Harabasz Index

- Davies-Bouldin Index

4. Visualizations

- Scatter Plot of Clusters (PCA reduced)

- Dendrogram for Hierarchical Clustering

- Pairplot of clusters

- Feature Correlation Heatmap

- Elbow Method Plot for Optimal K Selection

## Results

A comparative analysis of clustering performance was done for different numbers of clusters (c=3,4,5). The results were tabulated in a CSV file (clustering_results.csv) and analyzed using multiple performance metrics.

## Files

- *clustering_analysis.ipynb* – Python notebook containing the complete clustering analysis

- *clustering_results.csv* – Output file storing performance metrics

## Conclusion

The study provides an in-depth analysis of different clustering techniques applied to the UCI Wine dataset. K-Means performed efficiently, while Hierarchical clustering offered better interpretability. The Mean-Shift algorithm dynamically determined cluster centers but showed inconsistent results.

- Further improvements could include:

1.Trying other clustering algorithms like DBSCAN or Gaussian Mixture Models

2.Using additional dimensionality reduction techniques

3. Applying hyperparameter tuning for better clustering performance

