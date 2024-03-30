# What is it?

*Correlation* is a [[Statistical Measure]] that measures the **direction and strength** of the **linear relationship** between two numerical variables, meaning these two variables **change together at a constant rate**. 

*Correlation* is a great for **describing simple relationships** between variables without making a statement about cause and effect. Even though two variables can be highly correlated, **it doesn't imply causation**.

![[Correlation comic.png|600]]

___
# Notation and Definition

The first thing to have in mind when thinking about **correlated variables**, is that the concept of *correlation* **applies only to linear relationships**. More complex, non-**linear relationships** are **not explained by correlation**. 

*Correlation* is used in numerical format through a *correlation coefficient*, which is a [[Statistical Measure]] with values ranging from $-1$ to $+1$, normally written as $r$.

There are various to calculate a *correlation coefficient*, depending on the **type of data**, whether being a **ordinal**, **categorical** or **real-valued**. The most commonly used *coefficients* are [Pearson's](https://en.wikipedia.org/wiki/Pearson_correlation_coefficient) and [Spearman's](https://en.wikipedia.org/wiki/Spearman%27s_rank_correlation_coefficient).
___
## Pearson's Correlation Coefficient

*Pearson's Correlation Coefficient*, also called *bivariate correlation*, is the most used *correlation coefficient*, and any that someone talks about *correlation*, one should assume they are talking about *Pearson's*.

It evaluates **linear relationships** between **two continuous variables**, where a change is one variable relates to a **proportional change** in the other variable. The main takeaway is that it **only applies to linear relationships**.

Given $n$ as the number of data point **pairs**, $\sigma$ as the **standard deviation** and $x, y$ as the variables to correlate,  and $\overline{x}, \overline{y}$ as the **average** of said variables, one can calculate *Pearson's correlation* using the formula:
$$
r = \frac{1}{n-1} 
\sum^n_{i=1} 
\left(\frac{x_i - \overline{x}}{\sigma_x} \right)
\left(\frac{y_i - \overline{x}}{\sigma_y} \right)
$$
> [!tip] Using $r$ to calculate changes
> This will result in $r \in [-1, 1]$, where a change in a variable will result in $(\text{change value} * r)$ in the other variable. 

![[Correlation examples.png]]