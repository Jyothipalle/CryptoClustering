# CryptoClustering
Preparing the Data
Using the StandardScaler() module from scikit-learn to normalize the data from the CSV file.

Created a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.


Finind the best value for k 


Code the elbow method algorithm to find the best value for k. Use a range from 1 to 11. 

To visually identify the optimal value for k, plot a line chart of all the inertia values computed with the different values of k. 

 The best value for k is 4


 # Cryptocurrencies with K-Means by Using the Original Data 

Initialized the K-means model with four clusters by using the best value for k as 4

Fit the K-means model by using the original data. 

Predict the clusters for grouping the cryptocurrencies by using the original data. Reviewed the resulting array of cluster values. 

Created a copy of the original data, and then add a new column of the predicted clusters. 

Using hvPlot, created a scatter plot by setting x="price_change_percentage_24h" and y="price_change_percentage_7d". Color the graph points with the labels that you found by using K-means. Then added the crypto name to the hover_cols parameter to identify the cryptocurrency that each data point represents

# Optimize Clusters with Principal Component Analysis.

Created a PCA model instance, and set n_components=3.

Use the PCA model to reduce the features to three principal components. 

# explained variance 

 The total explained variance of the three principal components is 0.89503166 (Sum of all three)

Created a new DataFrame with the PCA data.

# Find the Best Value for k by Using the PCA Data 


Coded the elbow method algorithm, and used the PCA data to find the best value for k. Using  a range from 1 to 11. 

To visually identify the optimal value for k, plot a line chart of all the inertia values computed with the different values of k. 

The best value for k when using the PCA data is 4 .

 it differ from the best valueof k that  found by using the original data

# Cluster the Cryptocurrencies with K-means by Using the PCA Data 


Initialize the K-means model with four clusters by using the best value for k.

Fit the K-means model by using the PCA data. 

Predict the clusters for grouping the cryptocurrencies by using the PCA data. Review the resulting array of cluster values.

Create a copy of the DataFrame with the PCA data, and then add a new column to store the predicted clusters. 

Using hvPlot, created a scatter plot by setting x="PC1" and y="PC2". Color the graph points with the labels that you found by using K-means. Then add the crypto name to the hover_cols parameter to identify the cryptocurrency that each data point represents. 

# Visualize and Compare the Results 


Create a composite plot by using hvPlot and the plus sign (+) operator to compare the elbow curve that created from the original data with the one that created from the PCA data. 

Created a composite plot by using hvPlot and the plus (+) operator to compare the cryptocurrency clusters that resulted from using the original data with those that resulted from the PCA data. 

 # Based on visually analyzing the cluster analysis results


   Using fewer features to cluster means that the results are much more dispersed meaning that the clusters arent as accurate as when using more features.

code source : taken help from ASKBCS when i struck for few things here and there,otherthan that most of the assignemnt topic has learnt from class activity