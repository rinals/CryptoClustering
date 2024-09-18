# CryptoClusteringwith K-Means and PCA

### Project Overview
This project applies **K-Means clustering** to a cryptocurrency dataset to identify clusters of cryptocurrencies based on their price movements. To improve clustering performance, **Principal Component Analysis (PCA)** is used to reduce the dimensionality of the data, which helps remove noise and redundant features. The results are compared to assess the impact of using fewer features in the clustering process.

### Methodology

1. **Data Preprocessing**:
   - The cryptocurrency dataset was loaded and scaled using standardization to ensure all features contributed equally to the clustering process.
   - **Principal Component Analysis (PCA)** was applied to reduce the dimensionality of the data from its original feature set to 3 principal components, while retaining most of the variance in the data. This step helps reduce noise and computational complexity.

2. **K-Means Clustering**:
   - K-Means clustering was performed on both the **original scaled data** and the **PCA-transformed data**.
   - The **Elbow Method** was used to identify the optimal number of clusters (\( k \)) by plotting the inertia for different \( k \) values (1-11). The elbow point, where the inertia starts decreasing more slowly, was identified at \( k = 4 \).

3. **Visualization**:
   - **Elbow Curve Comparison**: Two Elbow curves were plotted—one for the original data and one for the PCA-transformed data. This helped visually confirm that the optimal \( k \) is consistent between the two datasets.
   - **Cluster Visualization**: Scatter plots were created to compare the clusters formed using the original features and the PCA-reduced features. The clusters from the PCA data showed clearer separation and more compact groupings, indicating improved clustering performance.

### Key Results
- **Optimal Number of Clusters**: The Elbow Method identified \( k = 4 \) as the optimal number of clusters for both the original and PCA-transformed data.
- **Impact of PCA**: 
  - PCA reduced the dataset's dimensionality, improving clustering by removing noise and irrelevant information.
  - The clusters formed from PCA-reduced data were more compact and distinct, with clearer boundaries compared to those formed from the original data.

### Conclusion
This project demonstrates the effectiveness of combining PCA with K-Means clustering to enhance the clarity and performance of clustering. By reducing the dimensionality of the data, PCA helps remove irrelevant features, leading to more distinct and well-separated clusters. Despite reducing the number of features, the key patterns in the data were preserved, and the clustering results remained robust.

### Dependencies
- **Python 3.x**
- **Pandas**
- **Scikit-learn**
- **hvPlot**

### How to Run
1. Load the cryptocurrency data and scale the features.
2. Apply **PCA** to reduce the data to 3 principal components.
3. Run **K-Means clustering** on both the original and PCA-transformed data.
4. Use the **Elbow Method** to find the optimal \( k \), and visualize the clusters using scatter plots.

### Contact
Rinal Shastri - rinal.shastri@outlook.com, rinaljoginshastri@gmail.com

### Acknowledgements
Module exercises, Xpert Learning Assistant, Chat GPT.
