# What is it?

A *binary tree* is a **hierarchical** [[Data Structures|Data Structure]] in which each element has **at most two children**, referred as left and right children. It's widely used for **storing**, **searching**, and **sorting** data.

Each *binary tree* has three items, the **data item**, the **address of the left child** and the **address of the right child**.

![[binary tree.png]]
___
# Characteristic 

To calculate the [[Big-O Notation]] of a *binary tree*, we use the *height* of the *tree*. The *height* is given by the difference of the *root level*, which is **always equal to $0$**, and the **desired element level**.

We can get the **maximum number of elements** at a given level by using a simple rule. Given $N$ as the **number of elements**, and $h$ the **depth of the tree**, $N_h = 2^{h + 1} - 1$.