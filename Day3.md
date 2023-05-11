## HTML Headings
* HTML headings are defined with the `<h1>` to `<h6>` tags.

* `<h1>` defines the most important heading. `<h6>` defines the least important heading.
# heading 1
## heading 2 
### heading 3
#### heading 4
##### heading 5
###### heading 6
>`<h1>Heading 1</h1>`
## Headings Are Important
* Search engines use the headings to index the structure and content of your web pages.
* `<h1>` headings should be used for main headings, followed by `<h2>` headings, then the less important `<h3>`, and so on.
* Each HTML heading has a default size. However, you can specify the size for any heading with the style attribute, using the CSS font-size property:
>`<h1 style="font-size:60px;">Heading 1</h1>`

* __Note__: Use HTML headings for headings only. Don't use headings to make text __BIG__ or __bold__.

## HTML Paragraphs
* The HTML `<p>` element defines a paragraph.

* A paragraph always starts on a new line, and browsers automatically add some white space (a margin) before and after a paragraph.

## HTML Horizontal Rules
* The `<hr>` tag defines a thematic break in an HTML page, and is most often displayed as a horizontal rule.

* The `<hr>` element is used to separate content (or define a change) in an HTML page.
* The `<hr>` tag is an empty tag, which means that it has no end tag.
>`<hr>`
## HTML Line Breaks
* The HTML `<br>` element defines a line break.
* Use `<br>` if you want a line break (a new line) without starting a new paragraph.
* The `<br>` tag is an empty tag, which means that it has no end tag.
>`<br>`
## The HTML `<pre>` Element
* The HTML `<pre>` element defines preformatted text.

* The text inside a `<pre>` element is displayed in a fixed-width font (usually Courier), and it preserves both spaces and line breaks:

```
<pre>
  My Bonnie lies over the ocean.

  My Bonnie lies over the sea.

  My Bonnie lies over the ocean.

  Oh, bring back my Bonnie to me.
</pre>
```
## The HTML Style Attribute
* Setting the style of an HTML element, can be done with the style attribute.

* The HTML style attribute has the following syntax:

>`<tagname style="property:value;">`
* The property is a CSS property. The value is a CSS value.
## Background Color
* The CSS `background-color` property defines the background color for an HTML element.
* Set the background color for a page to red:
>`<body style="background-color:red;">`

* Set background color for two different elements:


>`<h1 style="background-color:powderblue;">This is a heading</h1>`
>`<p style="background-color:tomato;">This is a paragraph.</p>`



## Text Color
* The CSS `color` property defines the text color for an HTML element:

>`<p style="color:blue;">This is a heading</p>`
>`<p style="color:red;">This is a paragraph.</p>`

## Fonts
* The CSS `font-family` property defines the font to be used for an HTML element:

>`<p style="font-family:verdana;">This is a paragraph1.</p>`
>`<p style="font-family:courier;">This is a paragraph2.</p>`

## Text Size
* The CSS `font-size` property defines the text size for an HTML element:

>`<p style="font-size:300%;">This is a paragraph1.</p>`
<p style="font-size:160%;">This is a paragraph2.</p>
Text Alignment
The CSS text-align property defines the horizontal text alignment for an HTML element:

## Text Alignment
* The CSS `text-align` property defines the horizontal text alignment for an HTML element:
>`<p style="text-align:left;">Left paragraph1.</p>`
>`<p style="text-align:center;">Centered paragraph2.</p>`
>`<p style="text-align:right;">Right paragraph3.</p>`

## HTML Formatting Elements
* Formatting elements were designed to display special types of text:

* `<b> - Bold text`
* `<strong> - Important text`
* `<i> - Italic text`
* `<em> - Emphasized text`
* `<mark> - Marked text`
* `<small> - Smaller text`
* `<del> - Deleted text`
* `<ins> - Inserted text`
* `<sub> - Subscript text`
* `<sup> - Superscript text`

## HTML `<b>` and `<strong>` Elements
* The HTML `<b>` element defines bold text, without any extra importance.

>`<b>This text is bold</b>`
* The HTML `<strong>` element defines text with strong importance. The content inside is typically displayed in bold.

* `<strong>`This text is important!`</strong>`

## HTML `<i>` and `<em>` Elements
* The HTML `<i>` element defines a part of text in an alternate voice or mood. The content inside is typically displayed in italic.

* __Tip:__ The `<i>` tag is often used to indicate a technical term, a phrase from another language, a thought, a ship name, etc.

>`<i>This text is italic</i>`
* The HTML `<em>` element defines emphasized text. The content inside is typically displayed in italic.

* __Tip:__ A screen reader will pronounce the words in `<em>` with an emphasis, using verbal stress.

>`<em>This text is emphasized</em>`
## HTML `<small>` Element
* The HTML `<small>` element defines smaller text:

>`<small>This is some smaller text.</small>`
## HTML `<mark>` Element
* The HTML `<mark>` element defines text that should be marked or highlighted:

>`<p>Do not forget to buy <mark>milk</mark> today.</p>`

## HTML `<del>` Element
* The HTML `<del>` element defines text that has been deleted from a document. Browsers will usually strike a line through deleted text:
~~example~~

>`<p>My favorite color is <del>blue</del> red.</p>`

## HTML `<ins>` Element
* The HTML `<ins>` element defines a text that has been inserted into a document. Browsers will usually underline inserted text:

>`<p>My favorite color is <del>blue</del> <ins>red</ins>.</p>`
## HTML `<sub>` Element
* The HTML `<sub>` element defines subscript text. Subscript text appears half a character below the normal line, and is sometimes rendered in a smaller font. Subscript text can be used for chemical formulas, like H$_2$O:

>`<p>This is <sub>subscripted</sub> text.</p>`

## HTML `<sup>` Element
* The HTML `<sup>` element defines superscript text. Superscript text appears half a character above the normal line, and is sometimes rendered in a smaller font. Superscript text can be used for footnotes, like WWW^[1]^, 25^125^:

>`<p>This is <sup>superscripted</sup> text.</p>`
