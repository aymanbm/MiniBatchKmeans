# Comparison of K-Means and Mini-Batch K-Means for Mall Customer Segmentation
This project aims to compare the performance of K-Means and Mini-Batch K-Means clustering algorithms in segmenting customers of a mall based on their purchasing behavior. By analyzing the patterns in customer data, we aim to identify distinct customer segments that can help tailor marketing and sales strategies.

## Objective
The goal is to compare the clustering results of K-Means and Mini-Batch K-Means, highlighting their strengths, weaknesses, and suitability for this type of clustering task. Specifically, we assess how each algorithm performs in terms of:

Speed (especially with large datasets)

Quality of clusters

Convergence behavior

## Dataset Overview
The dataset used in this project is the Mall Customers dataset, which includes the following features:

CustomerID: Unique identifier for each customer

Age: Age of the customer

Annual Income (k$): Customer's annual income (in thousands of dollars)

Spending Score (1-100): A score assigned by the mall based on the customer’s spending behavior

## Data Preparation
Preprocessed the dataset by handling missing values and standardizing numerical features like Age, Annual Income, and Spending Score.

Scaled the features to ensure all variables contribute equally to the clustering process.

Performed exploratory data analysis (EDA) to visualize the distribution of customers' features and look for patterns in the data.

## Models Compared
K-Means
K-Means is the classic clustering algorithm where the number of clusters, K, is specified in advance.

It works by iteratively assigning data points to the nearest cluster centroid and updating the centroid positions based on the mean of the points in each cluster.

Mini-Batch K-Means
Mini-Batch K-Means is a variant of the K-Means algorithm designed to be more efficient with large datasets.

It uses small random samples (mini-batches) of data to update the centroids, reducing computational cost and speeding up convergence.

## Model Evaluation
The clustering results were evaluated using the following metrics:

Silhouette Score: To measure the quality of the clustering by comparing the distance between points in the same cluster and points in different clusters.

Cluster Visualization: Using 2D plots (e.g., PCA or t-SNE) to visually compare the clusters formed by both algorithms.

## Results and Discussion
K-Means: We evaluated the clustering results in terms of both quality and speed. While it provides a strong clustering solution, it may be slower with larger datasets due to the iterative nature of the algorithm.

Mini-Batch K-Means: This algorithm was found to be faster, especially with large datasets, and still produces good-quality clusters, though it may require more careful tuning of the batch size.

## Installation & Setup

Ensure you have Python installed along with the required libraries.

Install dependencies using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
