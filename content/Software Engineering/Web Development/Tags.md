*Tags* are used in [[HTML]] to define different *elements* and the structure of web pages. Each *tag* **represents a different *element***.
___
## Declaring the HTML file

All [[HTML]] files should have an *.html* extension **and** start with the `<!DOCTYPE` declaration. It **defines to the browser what document type to expect**.

The **root tag** `<html>` is used to **create the container which all other elements will be inside of**, except for the `<DOCTYPE>` tag. It's a **good practice to specify the language** of the web site inside the `<html>` tag.

```html
<!DOCTYPE html>
<html lang="en"><!--HTML content--></html>
```

The **metadata tag** `<head>` is used to **define metadata**, being followed by the `<body>` which define the **document's body** and all that **will be seen by the user**.

The **`<head>`  tag** requires the **title element**, which is defined by the **title tag**, `<title>`. Still, it can **accept other metadata tags**, like `<style>`, `<base>`, `<meta>`, `<link>`, `<script>`, and `<noscript>`.

```html
<!DOCTYPE html>  
<html lang="en">

<head>
	<meta charset="utf>
	<title>Title of the document</title>
</head>

<body></body>
</html>
```

____
## Commenting in HTML

The **comment tag** `<!-- -->` is used to **create a comment** inside a [[HTML]] file, **without being interpreted** by the browser. It can either be a line comment, or span multiple lines.

```html
<!-- This is a comment and will not be rendered -->
<html><body><h1>This is rendered</h1></body></html>
<!--
This is a multi-line comment,
and will also not be rendered.
-->
```
___
## Titles and heading

The **heading tag** `<h1>` is used to **create headings and titles**, and it goes from `<h1>` to `<h6>`, with a **decreasing size** between each one.

```html
<h1>Title 1</h1>
<h2>Title 2</h2>
<h3>Title 3</h3>
<h4>Title 4</h4>
<h5>Title 5</h5>
```

Because *Obsidian* supports [[HTML]] content natively, we can run the example above and see its result:
<h1>Title 1</h1> <h2>Title 2</h2> <h3>Title 3</h3> <h4>Title 4</h4>
___
