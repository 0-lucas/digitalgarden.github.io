# What is it?

In [[Machine Learning]], the *silhouette score* is a metric used for [[Clustering]] algorithms, using the mean *silhouette coefficient* of all data samples, which **does not need labeled data**.

>[!tip] The differential of the *silhouette score*
> Most metrics for [[Clustering|clustering]] algorithms need *labeled data*, which for [[Clustering|clustering]] problems, the dataset will not contain any *label* for the data.
> Instead, *silhouette score* **demands only features data** and the **predicted clusters**.

However, *silhouette score* can present **inaccurate scores** for *clusters* which are **not spherical shaped**.
It only considers the **mean distance of a single sample**, while **not taking into account** information about **other samples**. This leads to abstract shapes which can have **better clusters**, but **worse scores**.
___
