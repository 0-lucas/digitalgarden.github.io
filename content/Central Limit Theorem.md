# What is it?

The *Central Limit Theorem* is a important **[[Limits|limit]] theorem** in [[Statistics]] and [[Probability]], which creates the base for **assuming characteristics from a sample to the entire population**, along with the [[Law of Large Numbers]].

The idea is that the **sum of a large number of averages is approximately normal**, given some assumptions. So for an unknown variable, one could use the *central limit theorem* to analyze it as a [[Normal Distribution]], which opens up various different methods to apply, like [[ANOVA]].
___
# Assumptions of the theorem

In order to apply the *central limit theorem*, some conditions must be met:

- ##### The variable must be *i.i.d.* - independent and identically distributed.
- ##### The population's distribution must have **finite variance**.
- ##### Sampling must be random and sufficiently large. The rule of thumb is $n \geq 30$,
- ##### Some statisticians also say that the sample size cannot be greater than 10% of the population.
___
# Applying the theorem

It's possible to apply the *central limit theorem* to any variable that **comply with the assumptions** above. The **original distribution of the variable doesn't really matter** as long as it follows the assumptions. 

Even though one can apply the *central limit theorem* conceptually, here's the step-by-step:

- ##### Write the variable of interest, $Y$ as the sum of $n$ *i.i.d* variable $X_i$'s:
$$
Y = X_1 + X_2 +...+X_n
$$
- ##### Find the expectation $EY$ and variance $Var(Y)$, noting that:
$$\begin{align}
&EY = n\mu, \quad Var(Y) = n\sigma^2 \\
&\text{where} \ \ \mu=EX_i, \quad \sigma^2 = Var(X_i)
\end{align}$$
- ##### To find $P(y_1 \leq Y \leq y_2)$, one can follow:
$$
\begin{align}

&P(y_1 \leq Y \leq y_2) = P\left(
\frac{y_1 - n\mu}{\sqrt{n}\sigma} \leq \frac{Y - n\mu}{\sqrt{n}\sigma} \leq \frac{y_2 - n\mu}{\sqrt{n}\sigma}
\right)
\\
& \approx \phi\left(\frac{y_2 - n\mu}{\sqrt{n}\sigma}\right) - \phi\left(\frac{y_1 - n\mu}{\sqrt{n}\sigma}\right)
\\ \\
&\text{where } \phi \text{ is the standard normal CDF.}\\ 
\end{align}
$$
\phi\left(\frac{y_2 - n\mu}{\sqrt{n}\sigma}\right)