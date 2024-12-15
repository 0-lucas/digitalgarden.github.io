# What is it?

In [[Statistics]], *inference* and *prediction* are **slightly different** results, that use similar methods, ranging from [[Statistical Modelling]] to [[Machine Learning]], to **achieve its desired output**.
However, **both can be summed** using the same formula:
$$
\hat{Y} = \hat{f}(X) + \epsilon
$$
Where $\hat{f}$ represents the **estimate of the true function** $f$, and $\hat{Y}$ the **resulting prediction** of $Y$.
___
## Inference

*Inference* 

___
## Prediction

*Prediction* can be summed up to a single, fully practical question:
	*having the right information and characteristics, can i predict a result of something?*

In *prediction*, $\hat{f}$ is treated like a *black box*. This means that is **not valuable** to **deeply understand** the relationship between a feature and its impact on the output variable. The **desired output** of a *prediction* problem, however, is to **accurately estimate $Y$**.
The **form or any method used to determine** $\hat{f}$ is generally **not of concern**, provided that $\hat{Y}$ is **close enough** to $Y$.