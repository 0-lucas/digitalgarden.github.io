# What is it?

In [[Machine Learning]], the *silhouette score* is a metric used for [[Clustering]] algorithms, using the mean *silhouette coefficient* of all data samples, which **does not need labeled data**.

The *silhouette coefficient* measures **how well each data point fits** into its *cluster*. It 

## Why silhouette score?

Most metrics for [[Clustering|clustering]] algorithms need *labeled data*, which for [[Clustering|clustering]] problems, the dataset will not contain any *label* for the data.
Instead, *silhouette score* **demands only features data** and the **predicted clusters**.
This **differs** from **other metrics** used for [[Clustering|clustering]] algorithms, which needs *true labels* for evaluation.
## The shortcoming of silhouette score

*Silhouette score* can present **inaccurate scores** for *clusters* which are **not spherical shaped**.
It only considers the **mean distance of a single sample**, while **not taking into account** information about **other samples**. This leads to *clusters* with *abstract shapes* that can have **better [[Clustering|clustering]]**, but **worse scores**.

![[silhouette vs dbcv score.png]]
___
# 