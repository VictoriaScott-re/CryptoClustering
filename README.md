# Cryptocurrency Clustering with K-Means

This project explores the use of K-Means clustering to analyze and group cryptocurrencies based on their price changes over various time periods. The analysis is performed on both the original dataset and a dimensionally-reduced version of the dataset using Principal Component Analysis (PCA).

## Project Overview

The goal of this project is to identify patterns and group similar cryptocurrencies by analyzing their price changes. By using K-Means clustering, we can classify cryptocurrencies into distinct groups based on their performance.

### Key Features

- **Data Normalization:** Standardizes the dataset using `StandardScaler` to ensure that all features contribute equally to the clustering process.
- **Elbow Method:** Utilized to determine the optimal number of clusters (`k`) by analyzing the inertia for different values of `k`.
- **Principal Component Analysis (PCA):** Reduces the dimensionality of the data, simplifying the clustering process while retaining the most important features.
- **Cluster Visualization:** Visualizes the clusters using `hvPlot` to compare results from the original and PCA-transformed data.

## Files in the Repository

- **`Crypto_Clustering.ipynb`:** The Jupyter Notebook containing the code for loading data, preprocessing, clustering with K-Means, and visualizing the results.
- **`crypto_market_data.csv`:** The dataset containing price change data for various cryptocurrencies.
- **`README.md`:** The file you are reading now, providing an overview of the project.

## Instructions

To replicate the analysis, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/crypto-clustering.git

2. **Install the Required Libraries**
   ```bash
   pip install pandas scikit-learn hvplot jupyterlab

4. ** Run the Jupyter Notebook**
   ```bash
   jupyter lab

## Results

- **Optimal Clusters:** The analysis determined that the optimal number of clusters (`k`) is 4 for both the original and PCA-transformed data.
- **Impact of PCA:** PCA reduced the dataset to three principal components, which simplified the clustering process and made the clusters more distinct, while still preserving around 89.5% of the original variance.
- **Visualization:** The resulting clusters are visualized in scatter plots, contrasting the differences between using the full set of features and the reduced PCA data.

## Conclusion

This project demonstrates the effectiveness of using PCA to simplify and enhance the clustering of cryptocurrencies. By reducing dimensionality, PCA allows for more efficient clustering while still capturing the most significant patterns in the data.
