# Customer Segmentation using K-Means Clustering

## Overview
This project demonstrates how to use **K-Means clustering** for customer segmentation. By analyzing customer demographic data such as **Age**, **Annual Income**, and **Spending Score**, we aim to group customers into distinct clusters. This segmentation allows businesses to target specific groups of customers with tailored marketing strategies and improve business operations.

## Project Structure
This repository contains the following files:
- **Customer_Segmentation_with_KMeans.ipynb**: The Jupyter Notebook containing the entire project with data preprocessing, clustering, and visualization.
- **requirements.txt**: List of dependencies used in this project for easy installation.
- **README.md**: The description and documentation for this project.

## Dataset
The dataset used in this project is the **Mall Customer Segmentation Data**. It consists of the following columns:
- **CustomerID**: A unique identifier for each customer.
- **Gender**: The gender of the customer (Male/Female).
- **Age**: Age of the customer.
- **Annual Income**: Annual income of the customer in thousands (k$).
- **Spending Score**: A score assigned by the mall based on customer behavior and spending.

You can download the dataset [here](https://raw.githubusercontent.com/vincentarelbundock/Rdatasets/master/csv/datasets/Mall_Customers.csv).

## Project Workflow

### 1. Data Preprocessing
- Load the dataset and check for any missing values.
- Convert categorical variables like **Gender** into numerical format using one-hot encoding.
- Standardize numerical features, such as **Age**, **Annual Income**, and **Spending Score**, for better performance of clustering algorithms.

### 2. Elbow Method for Optimal Clusters
- Use the **Elbow Method** to determine the optimal number of clusters. This method involves running K-Means for a range of cluster numbers and plotting the **inertia** (sum of squared distances) to identify the optimal number of clusters.

### 3. K-Means Clustering
- Implement the **K-Means algorithm** using the optimal number of clusters determined from the elbow plot.
- Cluster customers into distinct groups based on their purchasing behavior and demographic features.

### 4. Visualization of Clusters
- Use **matplotlib** and **seaborn** to visualize the clusters in 2D space.
- Create scatter plots to visually distinguish different clusters.

### 5. Cluster Analysis
- Perform analysis on the clusters by calculating the mean values of features (e.g., **Age**, **Annual Income**, and **Spending Score**) for each cluster.
- Identify key characteristics of each customer segment to assist in strategic decision-making.

## Key Insights
The K-Means clustering model identified distinct customer segments based on demographic and behavioral features. These clusters can be used for targeted marketing strategies:
- **Cluster 1**: Young customers with high spending.
- **Cluster 2**: Older customers with moderate income.
- **Cluster 3**: Customers with high income but low spending.
- **Cluster 4**: Low-income, low-spending customers.

## Requirements
To run this project, the following Python packages are required:

```bash
numpy
pandas
matplotlib
seaborn
scikit-learn
