# What is it?

In [[Statistics]], *one-way ANOVA* is a [[Statistical Modelling|statistical model]] which tests if **different samples are drawn from the same population**, taking into account **only one variable**. It's a subset of [[ANOVA]], applying it to a single variable.
___
# Calculating ANOVA

## Using Python

One could easily calculate the [[ANOVA]] table from multiples samples with a shared uni-variate variable using [[Python]]. The [[statsmodels]] library uses [[SciPy]] to easily return an [[ANOVA]] table.

```

```

___
## Calculating by hand

Normally, [[ANOVA]] it's not done by hand. It's too calculation-intensive. However, because *one-way ANOVA* uses only a single variable, one could follow the step-by-step to **understand the underlying algorithm**:

- #### Calculate each sample mean and the overall mean.
For each sample/ group present in the experiment, calculate its mean and then the overall mean, with all samples.

- #### Calculate the sum of squares, SS.
Given the **number of samples** $k$, the **sample mean** $\overline{x}$, and the **overall mean** as $\overline{X}$, calculate *SS*, sum of squares, of each sample and then sum them all. 
$$
SS = \sum_{i=1}^k (\overline{x}_i -\overline{X})^2
$$
- #### Calculate the squared error, SSE.
Similarly to [[Mean Squared Error]], calculate the **sum of squared errors** of each observation. Given $x_{ij}$ as **the $i^{th}$ observation in group $j$**, and $\overline{X}_j$ as the **mean of the group $j$**, and $n_j$ as the **number of observations of the sample**:
$$
SSE = \sum_{i=1}^{n_j} (x_{ij} - \overline{X}_j)^2
$$
- #### Calculate the total sum of squares, SST.
The **total sum of squares**, *SST*, is the sum of *SSE* and *SS*.
$$SST = SSE + SE$$
- #### Fill in the ANOVA table.
Now, just fill the [[ANOVA]] table with the metrics you just calculated.

| Source    | Sum of Squares(SS) | Degrees of Freedom(DF) | Mean Squares (MS) | F-statistic   |
| --------- | ------------------ | ---------------------- | ----------------- | ------------- |
| Treatment | SS                 | $k-1$                  | $SS / DF_t$       | $MS_t / MS_r$ |
| Residual  | SSE                | $n-k$                  | $SSE / DF_r$      |               |
| Total     | SST                | $n-1$                  |                   |               |
