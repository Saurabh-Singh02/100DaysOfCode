## How To Add CSS
* When a browser reads a style sheet, it will format the HTML document according to the information in the style sheet.

## Three Ways to Insert CSS
* There are three ways of inserting a style sheet:

* External CSS
* Internal CSS
* Inline CSS

## External CSS
* With an external style sheet, you can change the look of an entire website by changing just one file!
* External styles are defined within the `<link>` element, inside the `<head>` section of an HTML page:
```
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
```
* An external style sheet can be written in any text editor, and must be saved with a .css extension.
```
"mystyle.css"
body {
  background-color: lightblue;
}
```
`margin-left: 20px;`
* **Note:** Do not add a space between the property value (20) and the unit (px):
Incorrect (space): margin-left: 20 px;
Correct (no space): margin-left: 20px;

## Internal CSS
* Internal styles are defined within the `<style>` element, inside the `<head>` section of an HTML page:
```
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
```
## Inline CSS
* An inline style may be used to apply a unique style for a single element.
* To use inline styles, add the `style` attribute to the relevant element. The style attribute can contain any CSS property.
```
<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>
```

## Multiple Style Sheets
* If some properties have been defined for the same selector (element) in different style sheets, the value from the last read style sheet will be used. 

* If the internal style is defined after the link to the external style sheet, the `<h1>` elements will be "orange":
```
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
<style>
h1 {
  color: orange;
}
</style>
</head>
```
* However, if the internal style is defined before the link to the external style sheet, the `<h1>` elements will be "navy": 
```
<head>
<style>
h1 {
  color: orange;
}
</style>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```
## Cascading Order
* All the styles in a page will "cascade" into a new "virtual" style sheet by the following rules, where number one has the highest priority:

* Inline style (inside an HTML element)
* External and internal style sheets (in the head section)
* Browser default
* So, an inline style has the highest priority, and will override external and internal styles and browser defaults.

## CSS Comments
* Comments are used to explain the code, and may help when you edit the source code at a later date. Comments are ignored by browsers.

### Single line comment
/* This is a single-line comment */

### Multi line comment
/* This is
a multi-line
comment 
```
<head>
<style>
h1 {
  color: orange;
}
</style>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```
*/
