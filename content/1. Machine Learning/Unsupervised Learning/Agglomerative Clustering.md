# What is it?i

In [[Machine Learning]], *agglomerative [[Clustering|clustering]]* is a [[Unsupervised Learning]] [[Algorithms|algorithm]] for *hierarchical-based* [[Clustering|clustering]], meaning that it builds a [[Binary Trees|tree]] from the **leaves**, with each being a **single data point**, and then *clusters* these leaves until it **reaches a single cluster**, that is the **root of the tree**.
___
# How does it work?

The [[Algorithms|algorithm]] **supposes that all data points are *clusters***, and then, tries to **merge them together** until the desired number of *clusters* is reached.
Each step **merges the two nearest cluster to each other**. However, various method can be used to determine the nearness of two *clusters*.
\
## Metrics of nearness
Some **metrics used to determine nearness**, and available in [[scikit-learn]] are: [[Euclidean Distance]], [[Manhattan Distance]]