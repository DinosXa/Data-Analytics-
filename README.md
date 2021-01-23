# Data-Analytics-
Data Analyst Practitioner in  Business Analytics and Personalization Technologies


Examining real-time sales numbers and customer feedback, and performing customer segmentation via cluster analysis. 

This Operator performs clustering using the k-means algorithm. Clustering groups Examples together which are similar to each other. As no Label Attribute is necessary, Clustering can be used on unlabelled data and is an algorithm of unsupervised machine learning.

The k-means algorithm determines a set of k clusters and assignes each Examples to exact one cluster. The clusters consist of similar Examples. The similarity between Examples is based on a distance measure between them.

A cluster in the k-means algorithm is determined by the position of the center in the n-dimensional space of the n Attributes of the ExampleSet. This position is called centroid. It can, but do not have to be the position of an Example of the ExampleSets.

The k-means algorithm starts with k points which are treated as the centroid of k potential clusters. These start points are either the position of k randomly drawn Examples of the input ExampleSet, or are determined by the k-means++ heuristic if determine good start values is set to true.

All Examples are assigned to their nearest cluster (nearest is defined by the measure type). Next the centroids of the clusters are recalculated by averaging over all Examples of one cluster. The previous steps are repeated for the new centroids until the the centroids no longer move or max optimization steps is reached. Be aware that it is not ensured that the k-means algorithm converges if the measure type is not based on Euclidean Distance calculation (cause the recalculation of the centroids by averaging is assuming Euclidean space).

The procedure is repeated max runs times with each time a different set of start points. The set of clusters is delivered which has the minimal sum of squared distances of all Examples to their corresponding centroids.
