# K-Means-Clustering-Unsupervised-Learning
K-Means is one the most well-known and most commonly used algorithms for clustering due to its simplicity and speed. 
Parameters: https://scikit-learn.org/0.19/modules/generated/sklearn.cluster.KMeans.html
K-Means is one the most well-known and most commonly used algorithms due to its simplicity and speed. Although, at the same time, it has some limitations.
It is designed to make use of a few straightforward steps that are repeated through multiple iterations.

1.	The first step for the algorithm is to initialize a defined number of centroids (denoted as X’s in the chart).
2.	The distance between each point (vector) and each centroid is calculated, and then points are assigned to the nearest centroid.
3.	Each centroid is then assigned a new position based on the mean of all the points (vectors) in the same group (cluster).
4.	The process then repeats with points re-assigned based on new centroid positions and a new mean calculated, leading to new positions for centroids.
5.	The iterations continue until the centroids no longer change their position or the defined number of max iterations is reached.

K-Means uses the Euclidean distance between different points in space (vectors) to identify which ones belong together. Because of that, you also need to be aware of the following:
•	 You can only use numerical attributes in the K-Means algorithm. If you want to use categorical ones for your clustering, you will first need to convert them to numerical. There are multiple ways of doing this, such as using sklearn’s Ordinal Encoder or similar methods.
•	Be mindful of the scale and distribution of the attributes that you are using in your clustering. You may want to first exclude outliers by removing them or introducing “range caps.” You may also want to use Power Transformation or Min-Max scaling to transform and fit the distribution into the same range for each of your attributes.
•	Finally, depending on the type of your data and your use case, you may prefer to use a density-based algorithm instead of a distance-based one.

Density-Based Clustering refers to unsupervised machine learning methods that identify distinctive clusters in the data, based on the idea that a cluster/group in a data space is a contiguous region of high point density, separated from other clusters by sparse regions.

kmeans inertia_ attribute is: Sum of squared distances of samples #to their closest cluster center.
WCSS, inertia in sklearn is defined as the sum of the squared distance between each member of the cluster and its centroid.

Disadvantages:
•	K-Means is highly scale dependent and is not suitable for data of varying shapes and densities.
•	Evaluating results is more subjective. It requires much more human evaluation than trusted metrics.


