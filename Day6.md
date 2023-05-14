## HTML Block and Inline Elements
* Every HTML element has a default display value, depending on what type of element it is.

* There are two display values: block and inline.

## Block-level Elements
* A block-level element always starts on a new line, and the browsers automatically add some space (a margin) before and after the element.

* A block-level element always takes up the full width available (stretches out to the left and right as far as it can).

* Two commonly used block elements are: `<p>` and `<div>`.

* The `<p>` element defines a paragraph in an HTML document.

* The `<div>` element defines a division or a section in an HTML document.

* The `<p>` element is a block-level element.

* The `<div>` element is a block-level element.
```
<p>Hello World</p>
<div>Hello World</div>
```
* Here are the block-level elements in HTML:

``` 
<address> <article> <aside> <blockquote> 
<canvas> <dd> <div> <dl> <dt> 
<fieldset> <figcaption> <figure> <footer> 
<form> <h1>-<h6> <header> <hr> <li> 
<main> <nav> <noscript> <ol> 
<p> <pre> <section> <table>
<tfoot> <ul> <video>
```

## Inline Elements
* An inline element does not start on a new line.

* An inline element only takes up as much width as necessary.

* This is a `<span>` element inside a paragraph.

`<span>Hello World</span>`

## Here are the inline elements in HTML:

```
<a> <abbr> <acronym>
<b> <bdo> <big> <br>
<button> <cite> <code>
<dfn> <em> <i> <img>
<input> <kbd><label>
<map> <object> <output>
<q> <samp> <script> <select>
<small> <span> <strong> <sub>
<sup> <textarea> <time>
<tt> <var>
```

* __Note:__ An inline element cannot contain a block-level element!


* The `<div>` Element
* The `<div>` element is often used as a container for ***other HTML elements.***

* The `<div>` element has no required attributes, but style, class and id are common.

* When used together with CSS, the `<div>` element can be used to style blocks of content:

```
<div style="background-color:black;color:white;padding:20px;">
<h2>London</h2>
<p>London is the capital city of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
</div>
```

## The `<span>` Element
* The `<span>` element is an inline container used to mark up a part of a text, or a part of a document.

* The `<span>` element has no required attributes, but style, class and id are common.

* When used together with CSS, the `<span>` element can be used to style parts of the text:

```
<p>My mother has 
<span style="color:blue;font-weight:bold;">blue</span>
eyes and my father has 
<span style="color:darkolivegreen;font-weight:bold;">dark green</span>
eyes.</p>

```

## HTML `Iframes`
* An HTML iframe is used to display a web page within a web page.


## HTML `Iframe` Syntax
* The HTML `<iframe>` tag specifies an inline frame.

* An inline frame is used to embed another document within the current HTML document.

**Syntax**
`<iframe src="url" title="description"></iframe>`

* __Tip:__ It is a good practice to always include a title attribute for the `<iframe>`. This is used by screen readers to read out what the content of the iframe is.

## Iframe - Set Height and Width
* Use the height and width attributes to specify the size of the iframe.

* The height and width are specified in pixels by default:

```
<iframe src="demo_iframe.htm" height="200" width="300" title="Iframe Example"></iframe>
```
* Or you can add the style attribute and use the CSS height and width properties:

```
<iframe src="demo_iframe.htm" style="height:200px;width:300px;" title="Iframe Example"></iframe>
```

### Iframe - Remove the Border
* By default, an iframe has a border around it.

* To remove the border, add the style attribute and use the CSS border property:

```
<iframe src="demo_iframe.htm" style="border:none;" title="Iframe Example"></iframe>
```
* With CSS, you can also change the size, style and color of the iframe's border:

```
<iframe src="demo_iframe.htm" style="border:2px solid red;" title="Iframe Example"></iframe>
```

## Iframe - Target for a Link
* An iframe can be used as the target frame for a link.

* The target attribute of the link must refer to the name attribute of the iframe:

```
<iframe src="demo_iframe.htm" name="iframe_a" title="Iframe Example"></iframe>
```
```
<p><a href="https://www.w3schools.com" target="iframe_a">W3Schools.com</a></p>
```
## The HTML `<script>` Tag
* The HTML `<script>` tag is used to define a client-side script (JavaScript).

* The `<script>` element either contains script statements, or it points to an external script file through the src attribute.

* Common uses for JavaScript are image manipulation, form validation, and dynamic changes of content.

* To select an HTML element, JavaScript most often uses the document.getElementById() method.

* This JavaScript example writes "Hello JavaScript!" into an HTML element with id="demo":

```
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>
```
## The HTML `<noscript>` Tag
* The HTML `<noscript>` tag defines an alternate content to be displayed to users that have disabled scripts in their browser or have a browser that doesn't support scripts:

```
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>
<noscript>Sorry, your browser does not support JavaScript!</noscript>
```

## HTML - The Head Element
* The HTML `<head>` element is a container for the following elements: `<title>`, `<style>`, `<meta>`, `<link>`, `<script>`, and `<base>`.

## The HTML `<head>` Element
* The `<head>` element is a container for metadata (data about data) and is placed between the `<html>` tag and the `<body>` tag.

* HTML metadata is data about the HTML document. Metadata is not displayed.

* Metadata typically define the document title, character set, styles, scripts, and other meta information.

## The HTML `<title>` Element
* The `<title>` element defines the title of the document. The title must be text-only, and it is shown in the browser's title bar or in the page's tab.

* The `<title>` element is required in HTML documents!

* The content of a page title is very important for search engine optimization (SEO)! The page title is used by search engine algorithms to decide the order when listing pages in search results.

* The `<title>` element:

* defines a title in the browser toolbar
provides a title for the page when it is added to favorites
displays a title for the page in search engine-results
So, try to make the title as accurate and meaningful as possible!

* A simple HTML document:

```
<!DOCTYPE html>
<html>
<head>
  <title>A Meaningful Page Title</title>
</head>
<body>
```

* The content of the document......

```
</body>
</html>
The HTML <style> Element
The <style> element is used to define style information for a single HTML page:
```

```
<style>
  body {background-color: powderblue;}
  h1 {color: red;}
  p {color: blue;}
</style>
```

## The HTML `<link>` Element
* The `<link>` element defines the relationship between the current document and an external resource.

* The `<link>` tag is most often used to link to external style sheets:

`<link rel="stylesheet" href="mystyle.css">`

* __Tip:__ To learn all about CSS, visit our CSS Tutorial.

## The HTML `<meta>` Element
* The `<meta>` element is typically used to specify the character set, page description, keywords, author of the document, and viewport settings.

* The metadata will not be displayed on the page, but is used by browsers (how to display content or reload page), by search engines (keywords), and other web services.


**Define the character set used:**
`<meta charset="UTF-8">`

**Define keywords for search engines:**

`<meta name="keywords" content="HTML, CSS, JavaScript">`

**Define a description of your web page:**

`<meta name="description" content="Free Web tutorials">`

**Define the author of a page:**

`<meta name="author" content="John Doe">`

**Refresh document every 30 seconds:**

`<meta http-equiv="refresh" content="30">`

**Setting the viewport to make your website look good on all devices:**

`<meta name="viewport" content="width=device-width, initial-scale=1.0">`
* Example of `<meta>` tags:

```
<meta charset="UTF-8">
<meta name="description" content="Free Web tutorials">
<meta name="keywords" content="HTML, CSS, JavaScript">
<meta name="author" content="John Doe">
```
**Setting The Viewport**

* The viewport is the user's visible area of a web page. It varies with the device - it will be smaller on a mobile phone than on a computer screen.

* You should include the following `<meta>` element in all your web pages:

`<meta name="viewport" content="width=device-width, initial-scale=1.0">`

* This gives the browser instructions on how to control the page's dimensions and scaling.

* The width=device-width part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).

* The initial-scale=1.0 part sets the initial zoom level when the page is first loaded by the browser.

* Here is an example of a web page without the viewport meta tag, and the same web page with the viewport meta tag:

* __Tip:__ If you are browsing this page with a phone or a tablet, you can click on the two links below to see the difference.


## The HTML `<base>` Element
* The `<base>` element specifies the base URL and/or target for all relative URLs in a page.

* The `<base>` tag must have either an href or a target attribute present, or both.

* There can only be one single `<base>` element in a document!

* Specify a default URL and a default target for all links on a page:

```
<head>
<base href="https://www.w3schools.com/" target="_blank">
</head>

<body>
<img src="images/stickman.gif" width="24" height="39" alt="Stickman">
<a href="tags/tag_base.asp">HTML base Tag</a>
</body>
```
