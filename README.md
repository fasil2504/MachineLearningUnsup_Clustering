# MachineLearningUnsup_Clustering
KMeans Clustering and Hierarchical Clustering  used iris data set


The Iris flower data set or Fisher's Iris data set is a multivariate data set introduced by the British statistician, eugenicist, and biologist Ronald Fisher in his 1936 paper The use of multiple measurements in taxonomic problems as an example of linear discriminant analysis.[1] It is sometimes called Anderson's Iris data set because Edgar Anderson collected the data to quantify the morphologic variation of Iris flowers of three related species.[2] Two of the three species were collected in the Gaspé Peninsula "all from the same pasture, and picked on the same day and measured at the same time by the same person with the same apparatus".[3] Fisher's paper was published in the journal, the Annals of Eugenics, creating controversy about the continued use of the Iris dataset for teaching statistical techniques today.

This study we try to clustering Iris Dataset used Kmeans

Attribute Information:

sepal length in cm
sepal width in cm
petal length in cm
petal width in cm
class: -- Iris Setosa -- Iris Versicolour -- Iris Virginica


How KMeans Clustering Works
KMeans clustering is an unsupervised machine learning algorithm used to group a set of data points into distinct clusters based on their similarities. Here's a brief breakdown of how it works:

Initialization: The algorithm starts by randomly selecting K centroids, where K is the number of clusters desired.
Assignment Step: Each data point is assigned to the nearest centroid, forming clusters.
Update Step: The centroids are recalculated as the mean of all data points in each cluster.
Repeat: The assignment and update steps are repeated until the centroids no longer change or a maximum number of iterations is reached.
Why KMeans Clustering is Suitable for the Iris Dataset
The Iris dataset contains 150 samples of flowers, categorized into three species: setosa, versicolor, and virginica, based on four features (sepal length, sepal width, petal length, and petal width). KMeans clustering is suitable for this dataset because:

Natural Grouping: The Iris dataset contains inherent clusters (species of flowers), and KMeans aims to partition data into groups based on similarity, making it ideal for identifying these clusters.
Feature Space: The dataset has multiple numeric features, which KMeans uses effectively to calculate distances (typically Euclidean distance) and form clusters.
Dimensionality: With only four features, the dataset is relatively low-dimensional, making KMeans computationally efficient.
Three Classes: Since the number of species is known to be three, we can set K=3 for the KMeans algorithm, which aligns with the actual number of clusters in the data.




How Hierarchical Clustering Works
Hierarchical clustering is an unsupervised machine learning algorithm that builds a hierarchy of clusters either by:

Agglomerative Approach (Bottom-up):

Each data point starts as its own cluster.
Pairs of clusters are merged step by step based on some distance metric (e.g., Euclidean distance) until all data points are grouped into a single cluster or the desired number of clusters is reached.
Divisive Approach (Top-down):

All data points start in a single cluster.
The cluster is recursively split into smaller clusters until each data point forms its own cluster or a desired cluster count is reached.
A dendrogram is often used to visualize the hierarchy, showing how clusters merge or split at different distance levels.

Why Hierarchical Clustering is Suitable for the Iris Dataset
Flexible Cluster Formation: Hierarchical clustering does not require the user to predefine the number of clusters (unlike KMeans). The Iris dataset might exhibit a nested or hierarchical structure among the species, and hierarchical clustering can reveal this.

Visual Insight via Dendrogram: A dendrogram can give insights into how different species of flowers are related in terms of their feature similarities, showing potential subclusters within species.

Small Dataset: The Iris dataset contains only 150 samples, making it computationally feasible to perform hierarchical clustering. Hierarchical clustering can be computationally expensive for large datasets, but this is not a concern with Iris.

Natural Clustering: Similar to KMeans, the Iris dataset has natural clusters corresponding to the species of flowers. Hierarchical clustering can help detect these groupings without prior knowledge of the number of species.
