---
layout: default
title: "Rune.js Documentation"
---

<div id="logo"></div>

# Rune.js

Rune.js is a JavaScript library for programming graphic design systems with SVG. It features a chainable drawing API, an unobtrusive scene graph, and a range of features aimed specifically at graphic designers: native support for color conversion, grid systems, typography, pixel iteration, as well as an expanding set of computational geometry helpers. Oh, and it uses [virtual-dom](https://github.com/Matt-Esch/virtual-dom) under the hood.

## Getting started

First download the `rune.js` file and place it next to your HTML document. Then, add a link to the file in the `<head>` tag of the document.

```html
<head>
  <script type="text/javascript" src="rune.js"></script>
</head>
```

To start using the library, create a new file called `sketch.js` and add a link to this file inside the `<body>` tag of the document.

```html
<body>
  <script type="text/javascript" src="sketch.js"></script>
</body>
```

Finally, put the following code in `sketch.js` to create a new Rune object.

```js
var r = new Rune({
  container: "body",
  width: 500,
  height: 400
});
```

If you open the HTML file in your browser, you will see a blank page, as we haven't called any drawing functions yet. Add the following code to `sketch.js` and refresh your browser.

```js
r.rect(0, 0, 200, 200).fill(0, 0, 255);
```

You should now see a blue rectangle in the top-left corner of the screen. If stuck, [download the example project](#).

## Drawing shapes

### Shape

All shapes share some common functions. Here's an overview.

#### `.function(x, y, relative)`

This is something to say about this code example. It might be a little crazy, but that's how it is baby.

<script type="text/javascript" src="js/app.js"></script>