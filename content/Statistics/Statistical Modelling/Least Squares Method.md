# What is it?

The *least squares method* is a [[Mathematics|mathematical]] method used in [[Statistics]] and [[Machine Learning]] to **find the best-fitting line** of a set of data.
It's a method widely used for [[Linear Regression]] and other *regressive* [[Statistical Modelling|statistical models]], to find the **relation between variables** and **estimating outcomes**.

The objective is to **find a best-fitting line** based on the **deviation from all measured data points**, and the deviation itself is **measured with the squared error** $\epsilon^2$.

![[least squares line.png]]

____
# Applying the Least Squares method

We can use [[Linear Algebra]] concepts on collected data to find the **best-fitting line**. Given a set of data, we can map the **line function** $y = ax +b$ to the **known data of $x, y$**, and then we would discover the $a, b$ coefficients:

| X   | Y   |
| --- | --- |
| 1   | 2   |
| 2   | 3   |
| 3   | 2   |
| 4   | 4   |

$$
\begin{cases}
a + b = 2 \\
2a + b = 3 \\
3a + b = 2 \\
4a + b = 4
\end{cases} \qquad \text{rewritten as } \qquad
A
\begin{pmatrix}
1 & 1 \\
2 & 1 \\
3 & 1 \\
4 & 1 
\end{pmatrix}
*

\begin{pmatrix}
a \\
b
\end{pmatrix}
=
\begin{pmatrix}
2 \\
3 \\
2 \\
4
\end{pmatrix}
$$
