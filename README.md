# Lab11
In this project, I used K-Means clustering to segment credit card customers based on their usage behavior. Since the dataset did not contain labels or predefined groups, this was considered an unsupervised learning problem.

I started by importing the required libraries and loading the `CC_GENERAL.csv` dataset. Then, I explored the dataset using functions like `head()`, `info()`, and `describe()` to better understand the features and data types.

Next, I cleaned the data by removing the `CUST_ID` column because it only represents customer identification and does not help in clustering. I also checked for missing values and filled them using the mean of each column.

After preprocessing, I performed exploratory data analysis using histograms, scatter plots, and a correlation heatmap to understand customer behavior and relationships between features.

Before applying K-Means, I scaled the data using `StandardScaler` because the dataset contains features with different ranges, and scaling improves clustering performance.

To determine the optimal number of clusters, I used both the elbow method and silhouette score. Based on the results, I selected K = 4. Then, I trained the K-Means model and assigned cluster labels to each customer.

Finally, I analyzed the customer segments and visualized them using PCA. The results showed different customer groups such as low-spending customers, high-value active customers, and customers who rely more on cash advances. These insights can help companies create better marketing strategies and personalized services.
