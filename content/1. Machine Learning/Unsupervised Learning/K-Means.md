# What is it?

*K-Means* is a [[Machine Learning]] used in [[Unsupervised Learning]] and [[Clustering]] tasks. It can be easily implemented with [[scikit-learn]].
___
# Pseudo algorithm

```
Select and initialise K centroids

Repeat:
	For each data point:
		Assign to the nearest cluster

	For each centroid:
		Update coordinates

	Have centroids converged?
		Yes: stop iterating
		No: keep going
```