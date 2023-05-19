## What is CSS?
* CSS stands for Cascading Style Sheets
* CSS describes how HTML elements are to be displayed on screen, paper, or in other media
* CSS saves a lot of work. It can control the layout of multiple web pages all at once
* External stylesheets are stored in CSS files

## Why Use CSS?
* CSS is used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.

## CSS Syntax
```
h1 {
    color:green;
    font-size:20px;
}
```

![CSS Image](https://www.w3schools.com/css/img_selector.gif)

## CSS `Selectors`
* CSS selectors are used to "find" (or select) the HTML elements you want to style.

* We can divide CSS selectors into five categories:

* **Simple selectors** (select elements based on name, id, class)
* **Combinator selectors** (select elements based on a specific relationship between them)
* **Pseudo-class selectors** (select elements based on a certain state)
* **Pseudo-elements selectors** (select and style a part of an element)
* **Attribute selectors** (select elements based on an attribute or attribute value)

## The CSS element Selector
* The element selector selects HTML elements based on the element name.

* Here, all `<p>` elements on the page will be center-aligned, with a red text color: 
```
p {
  text-align: center;
  color: red;
}
```
## The CSS id Selector
* The id selector uses the id attribute of an HTML element to select a specific element.

* The id of an element is unique within a page, so the id selector is used to select one unique element!

* To select an element with a specific id, write a **hash (#)** character, followed by the id of the element.

* The CSS rule below will be applied to the HTML element with `id="para1"`: 
```
#para1 {
  text-align: center;
  color: red;
}
<p id="para1">This is the para1</p>
```
* **Note:** An id name cannot start with a number!


## The CSS class Selector
* The class selector selects HTML elements with a specific class attribute.

* To select elements with a specific class, write a **period (.) or dot** character, followed by the class name.

* In this example all HTML elements with `class="center"` will be red and center-aligned: 
```
.center {
  text-align: center;
  color: red;
}
<p class="center">This is a class selector</p>
```

* In this example only `<p>` elements with `class="center"` will be red and center-aligned: 

* HTML elements can also refer **to more than one class.**

* In this example the `<p>` element will be styled according to `class="center"` and to `class="large"`: 
```
<p class="center large">This paragraph refers to two classes.</p>
```
**Note:** A class name cannot start with a number!

## The CSS Universal Selector
* The universal selector **(*)** selects all HTML elements on the page.

* The CSS rule below will affect every HTML element on the page: 
```
* {
  text-align: center;
  color: blue;
}
```

## The CSS Grouping Selector
* The grouping selector selects all the HTML elements with the same style definitions.

* Look at the following CSS code (the h1, h2, and p elements have the same style definitions):
```
h1 {
  text-align: center;
  color: red;
}

h2 {
  text-align: center;
  color: red;
}

p {
  text-align: center;
  color: red;
}
```
* It will be better to group the selectors, to minimize the code.

* To group selectors, separate each selector with a **comma(,)**.

```
h1, h2, p {
  text-align: center;
  color: green;
}
```
