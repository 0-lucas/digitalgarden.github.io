# What is it?

In [[Machine Learning]], the *silhouette score* is a metric used for [[Clustering]] algorithms, using the mean *silhouette coefficient* of all data samples, which **does not need labeled data**.

The *silhouette coefficient* measures **how well each data point fits** into its *cluster*. It matches both **cohesion** *(how close a data point is to other points of its own cluster)*, and **separation** *(how far a data point is from points in other cluster)*.

___
## Why silhouette score?

Most metrics for [[Clustering|clustering]] algorithms need *labeled data*, which for [[Clustering|clustering]] problems, the dataset will not contain any *label* for the data.
Instead, *silhouette score* **demands only features data** and the **predicted clusters**.
This **differs** from **other metrics** used for [[Clustering|clustering]] algorithms, which needs *true labels* for evaluation.
## The shortcoming of silhouette score

*Silhouette score* can present **inaccurate scores** for *clusters* which are **not spherical shaped**.
It only considers the **mean distance of a single sample**, while **not taking into account** information about **other samples**. This leads to *clusters* with *abstract shapes* that can have **better [[Clustering|clustering]]**, but **worse scores**.

![[silhouette vs dbcv score.png]]
___
# Calculation

For a specific data point, its *silhouette coefficient* is calculated as:
$$
s_{i} = \frac{b_{i} - a_{i}}{\max (b_{i}, a_{i})}
$$
Where $b$ is **separation**, and $a$ is **cohesion**, which can be calculated for **each** data point as:
$$
\begin{align}
&a_{i} = \frac{1}{|C_{i}| - 1} \sum_{j \in C_{i}, i\neq j} d(i,j)
\end{align}
$$