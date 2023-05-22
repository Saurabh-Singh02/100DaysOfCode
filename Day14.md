## CSS Backgrounds
* The CSS background properties are used to add background effects for elements.

* background-color
* background-image
* background-repeat
* background-attachment
* background-position
* background (shorthand property)

## CSS background-color
* The background-color property specifies the background color of an element.
```
body {
  background-color: lightblue;
}
```
* With CSS, a color is most often specified by:
 * a valid color name - like "red"
 * a HEX value - like "#ff0000"
 * an RGB value - like "rgb(255,0,0)"

## Other Elements
* You can set the background color for any HTML elements:

* Here, the `<h1>`, `<p>`, and `<div>` elements will have different background colors: 
```
h1 {
  background-color: green;
}

div {
  background-color: lightblue;
}

p {
  background-color: yellow;
}
```

## Opacity / Transparency
* The opacity property specifies the opacity/transparency of an element. It can take a value from 0.0 - 1.0. The lower value, the more transparent:
```
div {
  background-color: green;
  opacity: 0.3;
}
```
8 **Note:** When using the opacity property to add transparency to the background of an element, all of its child elements inherit the same transparency. This can make the text inside a fully transparent element hard to read.

## Using RGBA
```
div {
  background: rgba(0, 128, 0, 0.3) /* Green background with 30% opacity */
}
```

## CSS background-image
* The background-image property specifies an image to use as the background of an element.

* By default, the image is repeated so it covers the entire element.
```
body {
  background-image: url("cat.gif");
}
```
```
body {
  background-image: url("dog.jpg");
}
```
* **Note:** When using a background image, use an image that does not disturb the text.

* The background image can also be set for specific elements, like the `<p>` element:
```
p {
  background-image: url("boy.gif");
}
```
