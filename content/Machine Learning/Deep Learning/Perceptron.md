# What is it?

A *perceptron* is the simplest [[Neural Networks|neural network unit]], being historically **modeled after a biological neuron**. Similar to the neuron, there are **signals flowing from the input to the output**. These *signals* interact with three properties: the *bias*, the *weight* and the [[Activation Functions|activation function]].

![[perceptron.png]]

Given, $f$ as the [[Activation Functions|activation function]], $w$ as the *weight* $x, y$ as the *input and output*, and $b$ as the bias, the *perceptron* can be mathematically represented as:

$$
y = f(w_ix_i + b) 
$$

Normally, we can **represent the set of inputs as [[Vectors]]**, and the product of $w * b$ becomes a *dot product*:

$$
y= f(\boldsymbol{wx} + b)
$$
# Implementing with PyTorch

One can easily implement a *perceptron* algorithm using [[PyTorch]]: