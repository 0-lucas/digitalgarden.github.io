# What is it?

In [[Machine Learning]], *clustering* is an [[Unsupervised Learning]] *task* which focuses on learning *patterns* and *structures* of a dataset, **grouping similar data points** into groups, often called *clusters*.

![[clustering.png]]
___
# Use cases

*Clustering* is a **flexible task** which can be used both as the **only model of a project**, or as a **processing step** for a later model.

- ##### Segmentation
	Given the need to **discover different segments or groups in a dataset**, one could apply *clustering* and then use the **output clusters** to perform any later analysis. *e.g. cluster customers and show different ads for each segment.*

- ##### Data analysis
	One could also apply *clustering* to the whole dataset, and then **analyze each cluster separately and differently**, depending on the objective.

- ##### [[Dimensionality Reduction]]
	Datasets with **too many features** can be **reduced** using *clustering* techniques. This process is called [[Dimensionality Reduction]].

- ##### Outlier / anomaly detection
	Any data point which **has no similarity** to the others or **doesn't properly fit into any cluster**, can be considered an [[Outlier]]. This method is commonly used to detect *fraudulent* instances.

 - ##### Semi-supervised learning
	When used with a badly labeled dataset, *clustering* can supplement another [[Machine Learning|ML]] algorithm **with labeled data** (which are the actual *clusters)*. This technique categorizes a [[Semi-Supervised Learning]] method.
___
# Algorithms

Probably the most used *clustering* algorithm is [[K-Means]].