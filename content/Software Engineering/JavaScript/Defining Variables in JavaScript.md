A variable in [[JavaScript]] can be defined using **three different keywords**, `let`, `var` and `const`, or automatically, which is a bad practice.

To declare a variable automatically, one could just **assign a value to it**. Because [[JavaScript]] is loosely typed, it will automatically assign a data type to it.

```javascript
x = "Hello world!";

console.log(x);
```
___
#  Using var

The `var` keyword was the **original way of declaring variables** until 2015, where the other keywords were introduced.
It's **not a good practice** to use it nowadays, and should be only used when **developing for older browsers and applications**.

```javascript
var x = "This is a var variable. Bad practice!!";

console.log(x);
```
___
# Using let and const

For most use cases, `const` should be **always preferred**. It creates an **immutable variable**, meaning it's value cannot be changed