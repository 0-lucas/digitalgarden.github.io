# What is it?

In a [[MVC]] application, the *controller* is the **layer responsible** for receiving all [[HTTP]] requests from the user, **interpreting it**, **requesting data from the [[Models|model]]**, and returning it to the [[Views|view]]. In other words, it connects the [[Views|view]] and the [[Models|model]].

![[mvc example.png]]
___
# ASP.NET Controllers

In [[ASP.NET]], a *controller* is a class derived from the `Microsoft.AspNetCore.Mvc.Controller` class, used to define a **set of related methods** called *actions*. An *action* is any **public method** defined inside the *controller*.