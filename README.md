# CryptoClustering

This project applies clustering techniques to a dataset of cryptocurrencies to identify distinct groups based on their performance metrics. Principal Component Analysis (PCA) is used to reduce the dimensionality of the data, and K-Means clustering is applied to group the cryptocurrencies.
I classify cryptocurrencies according to their price fluctuations across various timeframes. Specifically, you will examine price changes over intervals spanning 24 hours, 7 days, 30 days, 60 days, 200 days, and 1 year.
Project Structure

- Crypto_Clustering.ipynb: The main Jupyter notebook that contains the code for data loading, processing, PCA transformation, clustering, and visualization.
- crypto_market_data.csv: The dataset used in the project, containing various performance metrics for different cryptocurrencies.
- README.txt: This file, providing an overview and instructions for the project.

Requirements

- Python 3.7 or higher
- Required Python packages:
  - pandas
  - scikit-learn
  - matplotlib
  - hvplot

You can install the required packages using pip:

pip install pandas scikit-learn matplotlib hvplot

Instructions

1. Load and Prepare the Data

- The dataset (crypto_market_data.csv) is loaded into a DataFrame and pre-processed.
- StandardScaler is used to normalize the data.

2. Dimensionality Reduction with PCA

- PCA is applied to reduce the data to three principal components.
- The explained variance of each component is analyzed to understand its contribution.

3. Clustering with K-Means

- The Elbow method is used to determine the optimal number of clusters (k).
- K-Means is applied to the PCA-transformed data to group cryptocurrencies into clusters.
- The resulting clusters are analyzed and visualized.

4. Visualization

- Scatter plots are generated using matplotlib and hvPlot to visualize the clusters in the reduced PCA space.

Results

- The analysis shows that k=4 is the optimal number of clusters for the given data.
- The features price_change_percentage_1y, price_change_percentage_24h, and price_change_percentage_7d were identified as having the strongest influences on the principal components.

How to Run

1. Clone the repository:
   git clone https://github.com/your-username/cryptocurrency-clustering.git
   cd cryptocurrency-clustering

2. Open the Jupyter notebook (Crypto_Clustering.ipynb) and run the cells sequentially to reproduce the analysis.

Contributing

Contributions are welcome! Please open an issue or submit a pull request with your proposed changes.

License CU
