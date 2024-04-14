# What is it?

The *Law of Large Numbers* is a important **limit theorem** in [[Statistics]] and [[Probability]], which creates the base for **assuming characteristics from a sample to the entire population**.

The basic idea behind the *law of large numbers* is that if you **repeat an experiment independently, after some number of times, the average of all results should be close to the expected value of said experiment**. In other words, if you collect **more samples**, you will have a **better estimate**.

>[!tip] Averaging values to get better accuracy
> In general, one **can't just measure a process once** and determine that the measured value is a good estimate. Commonly, statisticians **measure a process a repeated number of times** and **average all values** to get said estimate, which is **less sensitive to uncontrolled variance** of the first case.

Some assumptions are made before applying the *law of large numbers*:
 - ##### Variables must be *i.i.d.* - independent and identically distributed.
 - ##### [[Variance]] should be finite.
___
# Weak law of large of numbers

The *weak law of large numbers* states that the **mean of the sample will converge in probability to the expected value** of its respective probability distribution, **as the number of samples goes to infinity**.

This can be mathematically translated to:
$$
\lim_{n\to\infty} P(|\overline{x}_n - \mu)
$$