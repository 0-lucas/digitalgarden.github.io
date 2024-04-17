# What is it?

In [[Statistics]], *one-way ANOVA* is a [[Statistical Modelling|statistical model]] which tests if **different samples are drawn from the same population**, taking into account **only one variable**. It's a subset of [[ANOVA]], applying it to a single variable.
___
# Calculating ANOVA

Normally, [[ANOVA]] it's not done by hand. It's too calculation-intensive. However, because *one-way ANOVA* uses only a single variable, one could follow the step-by-step to **understand the underlying algorithm**:

- #### Calculate each sample mean and the overall mean.
For each sample/ group present in the experiment, calculate its mean and then the overall mean, with all samples.

- #### Calculate the sum of squares, SS.
Calculate *SS*, the **sum of squares**, using the formula $/Sigma $