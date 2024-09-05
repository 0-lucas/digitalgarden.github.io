# What is it?

*K-Means* is a [[Machine Learning]] used in [[Unsupervised Learning]] and [[Clustering]] tasks. It can be easily implemented with [[scikit-learn]].
___
# How does it work?

The *K-Means* algorithm need the number of *centroids* **before initiating the learning phase**, meaning that it **should be decided by the *data scientist***, either **directly** or using **another algorithm to optimally retrieve** a possible best number of *centroids*.

>[!tip] What are *centroids*?
> A *centroid* is coordinate where the **cluster will be centered upon**, meaning that all data points will be **calculated in reference** to the *centroid*.
> It's also considered the *mean* of the *cluster*, once that *K-Means* place the output *centroids* as the **average of the distance between all instances** from the *cluster*

It's also possible to **preemptively determine the initial position** of the *centroids*, or to **randomly let the algorithm decide**.

Then, each data point is **assigned to each *cluster*** considering the **nearest *centroid***, and the *centroid* is recalculated. Then, if no *centroid* moved, then the algorithm **has reached convergence**.
	![[Pasted image 20240904214924.png]]
## Pseudo algorithm

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
