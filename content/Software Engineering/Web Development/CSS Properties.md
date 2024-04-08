A *CSS property* determine the **style of an element** using [[CSS]]. It has various different properties, referring to **position**, **border**, **text**, **color**, and so on.
___
# Coloring

[[CSS]] can be specified using **defined names**, ***RGB* values**, ***HEX* values**, and ***HSL* values**.

>[!tip] List of standardized color names
>All browsers support a list of 140 colors, each defined by **its own name**. You can access the list [clicking here](https://www.w3schools.com/colors/colors_names.asp).

___
## RGB coloring

*RGB* coloring can be done using the *(red, green, blue)* **syntax**. Each parameter defines the **intensity** of a color **between a range of 0 and 255**.
For example, an **intense red** can be given by the following *property*:

```css
* {
	color: rgb(255, 0, 0);
}
```
___
## Hex coloring

*HEX* coloring specifies an **hexadecimal color** with *`#RRGGBB`*, where the *red*, *green* and *blue* hexadecimal integers specify the **components of the color**, where `ff` is the **highest value**.
For example, an **intense blue** can be given by the following *property*:

```css
* {
	color: #0000ff
}
```
___
## HSL coloring

*HSL* coloring specifies the **hue**, **saturation**, and **lightness** of a color in the form `(0-360,0-100,0-100)`. 
For example, an **intense green** can be given by the following *property*:

```css
* {
	color: hsl(120, 100%, 50%)
}
```
___
## Formatting the background

We can use the *background-color property* to apply a **background color** to any *element*. If used for the `<body>` section, it applies to the **background of the entire page**.

The *background-image* is very similar, but it **applies a background image** instead of coloring it.

```css
body {
	background-color: blanchedalmond;
	color:blueviolet;
	/*background-image: url("doge.jpg");*/
}
```
___
# Box Model

[[CSS]] works with [[HTML]] wrapping *elements* with the *[[CSS]] box model*. It consists of **content**, **padding**, **border**, and **margin**.

![[css box model.png]]

Then, you can **specify each property and customize it**.
___
## Borders

The *borders* can be customized by specifying each border or by 