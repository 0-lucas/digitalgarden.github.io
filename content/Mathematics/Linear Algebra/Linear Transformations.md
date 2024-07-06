# What is it?

In [[Linear Algebra]], *linear transformations* (or *linear mapping*) are *functions* which **linearly transforms [[Matrices|matrices]] and [[Arrays|arrays]]** to different [[Vector Spaces]]. They are widely used in *graphical computing* to transform graphics and *engineering* to work with different physical structures.

![[linear transformatinos.png]]

In fact, [[Matrix Multiplication]] is a form of *matrix transformation* that can be characterized as a *linear transformation*, once it **transforms** a [[Matrices|matrix]] from $\mathbf{R}^n \to \mathbf{R^m}$ *linearly*, and the *function* can be thought as the *second multiplied [[Matrices|matrix]]*.
___
# How does it work?
A *linear transformation* $T: X \to W$can be [[Mathematics|mathematically]] denoted:

$$
\begin{align}
& T: \mathbf{R}^n \to \mathbf{R}^m \\

& T(x_{1}, x_{2},\dots, x_{n}) = (w_{1},w_{2},\dots w_{m}) \\
\end{align}

$$
Where $T$ is a *function* which transform any [[Vectors|vector]] $x \in \mathbf{R}^n$ to $w \in \mathbf{R}^m$, given that it **satisfies the following properties**:

$$
\begin{align}
&\text{}T(x + y) = T(x) + T(y) \\
&\text{and} \\
&T(ax) = aT(x)
\end{align}
$$

For transformations which **do not satisfy the above conditions**, it's **not characterized as a *linear transformation***.
___
# 