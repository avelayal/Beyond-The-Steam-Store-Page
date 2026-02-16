# Beyond the Store Page: Clustering Steam Games by Player Engagement and Pricing

Steam is among the largest PC game marketplaces; however, store information such as price and discounts does not fully capture player engagement. This study applies unsupervised machine learning to cluster Steam games based on pricing and engagement-related features, including playtime, ownership estimates, reviews, and popularity indicators.

To enhance clustering stability and reduce noise, Principal Component Analysis (PCA) was employed to reduce dimensionality while preserving at least 90% of the dataset’s variance. Multiple clustering algorithms were evaluated, including K-Means, Agglomerative Hierarchical Clustering, and Gaussian Mixture Models (GMM). According to internal evaluation metrics (Silhouette Score, Davies–Bouldin Index, and Calinski–Harabasz Index), K-Means yielded the most stable and interpretable results.

The final model concentrated on paid games with non-zero playtime, reduced the feature space to six principal components, and applied K-Means clustering with k = 3. This approach identified three interpretable clusters:

1. High-traction mainstream titles characterized by strong engagement and visibility
2. Heavily discounted games that still show moderate engagement
3. Long-tail low-traction titles with low engagement and limited community activity

Overall, the results show that clustering can reveal meaningful behavioral segments in the Steam marketplace using only pricing and engagement signals.

## Dataset
This project uses the following Kaggle dataset:  
https://www.kaggle.com/datasets/artermiloff/steam-games-dataset/data?select=games_march2025_cleaned.csv
