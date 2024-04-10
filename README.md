# CryptoClustering

Predicting if cryptocurrencies are affected by 24-hour or 7-day price changes.

Read Data:
Readcsv
![Screenshot 2024-04-10 at 4 26 56 pm](https://github.com/patricb98/CryptoClustering/assets/145084886/b0c4cf82-63f5-4045-8355-f79902618d7f)

Summary statistics 
![Screenshot 2024-04-10 at 4 28 55 pm](https://github.com/patricb98/CryptoClustering/assets/145084886/79d48654-db74-48ac-9cee-b1df70a8066d)

Plot dataframe
![Screenshot 2024-04-10 at 4 29 29 pm](https://github.com/patricb98/CryptoClustering/assets/145084886/2652fe20-5b5b-4479-8a9d-b1c51d6bba96)

Prepare Data:
Scaled Data
![Screenshot 2024-04-10 at 4 30 07 pm](https://github.com/patricb98/CryptoClustering/assets/145084886/f003d40c-44f7-49d6-bd3c-91cca6672cc2)

Find the Best Value for k Using the Original Data:
**Question:** What is the best value for `k`?
**Answer:** 4
![Screenshot 2024-04-10 at 4 43 27 pm](https://github.com/patricb98/CryptoClustering/assets/145084886/e7c2a61f-d700-4a7f-bf0a-77e4e456c248)

Cluster Cryptocurrencies with K-means Using the Original Data:
![Screenshot 2024-04-10 at 4 46 01 pm](https://github.com/patricb98/CryptoClustering/assets/145084886/0da3fd7d-ddae-4dc7-8f73-1b061dfe8e82)

Optimise Clusters with Principal Component Analysis:
**Question:** What is the total explained variance of the three principal components?
**Answer:** 88.86%

Find the Best Value for k Using the PCA Data:
**Question:** What is the best value for `k` when using the PCA data?
* **Answer:** 4
* **Question:** Does it differ from the best k value found using the original data?
* **Answer:** no the k value stays the same as the original data set, but the inertia value does change. The inertia value changes from 79.022 to 44.131. This change shows that the data points are closer together as the lower the inertia value the tigher the clusters. 
![Screenshot 2024-04-10 at 4 47 00 pm](https://github.com/patricb98/CryptoClustering/assets/145084886/644fcb97-94dd-4527-9fb2-81ccf57206a3)

Cluster Cryptocurrencies with K-means Using the PCA Data:
![Screenshot 2024-04-10 at 4 48 03 pm](https://github.com/patricb98/CryptoClustering/assets/145084886/7fc126ea-20a5-4f69-a422-23ff75f88d95)
 
**Question:** After visually analysing the cluster analysis results, what is the impact of using fewer features to cluster the data using K-Means?
* **Answer:** 
  
  Looking at the comparision between the elbow curves the elbow 2 (pca) has a lower inertia value. This means that using fewer features reduced the distance between the data points within the clusters(tighter clustering).

  Comparing the original data graph and pca data graph. Original Data graph has clusters that are overlapping (red 1 in blue 0 cluster). Compared to PCA Data graph which uses fewer features, the clusters are more defined and organised. 

  The advantage of using PCA method to reduce features results in well defined clusters, which can highlight patterns and produce more accurate results. 


