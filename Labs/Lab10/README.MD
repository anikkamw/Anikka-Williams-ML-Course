Lab 10: Unsupervised Learning (Clustering & PCA)

Overview: This lab focused on Unsupervised Learning, specifically how to discover hidden patterns in unlabeled data using K-Means Clustering and Principal Component Analysis (PCA).

What I Learned: I practiced the Elbow Method to determine the optimal number of clusters ($k=4$) for a synthetic customer dataset and utilized PCA to reduce the 4-dimensional Iris dataset down to 2 principal components for visualization.

What I Did: I implemented the KMeans and PCA algorithms from scikit-learn. My PCA model successfully explained 97.77% of the total variance in the Iris dataset using only two components, proving that the original four features were highly correlated.

Challenges: A key challenge was the "Elbow Method" interpretation; I learned that selecting the largest possible $k$ would minimize inertia but fail to identify meaningful groups, requiring a balance between mathematical precision and practical pattern discovery.
