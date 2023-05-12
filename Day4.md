## HTML `<blockquote>` for Quotations
* The HTML `<blockquote>` element defines a section that is quoted from another source.

* Browsers usually indent `<blockquote>` elements.


>`<p>Here is a quote from WWF's website:</p>`

>`<blockquote cite="http://www.worldwildlife.org/who/index.html">`
`For 60 years, WWF has worked to help people and nature thrive. As the world's leading conservation organization, WWF works in nearly 100 countries. At every level, we collaborate with people around the world to develop and deliver innovative solutions that protect communities, wildlife, and the places in which they live.`
`</blockquote>`

>For 60 years, WWF has worked to help people and nature thrive. As the world's leading conservation organization, WWF works in nearly 100 countries. At every level, we collaborate with people around the world to develop and deliver innovative solutions that protect communities, wildlife, and the places in which they live.

## HTML `<q>` for Short Quotations
The HTML `<q>` tag defines a short quotation.

* Browsers normally insert quotation marks around the quotation.
```
<p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>
```
## HTML `<abbr>` for Abbreviations
* The HTML `<abbr>` tag defines an abbreviation or an acronym, like "HTML", "CSS", "Mr.", "Dr.", "ASAP", "ATM".

* Marking abbreviations can give useful information to browsers, translation systems and search-engines.

* __Tip:__ Use the global title attribute to show the description for the abbreviation/acronym when you mouse over the element. 

`<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>`

## HTML `<address>` for Contact Information
* The HTML `<address>` tag defines the contact information for the author/owner of a document or an article.

* The contact information can be an email address, URL, physical address, phone number, social media handle, etc.

* The text in the `<address>` element usually renders in italic, and browsers will always add a line break before and after the `<address>` element.

```
<address>
Written by John Doe.<br>
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>
```
## HTML `<cite>` for Work Title
* The HTML `<cite>` tag defines the title of a creative work (e.g. a book, a poem, a song, a movie, a painting, a sculpture, etc.).

* Note: A person's name is not the title of a work.

* The text in the `<cite>` element usually renders in italic.

>`<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>`

## HTML `<bdo>` for Bi-Directional Override
* BDO stands for Bi-Directional Override.

* The HTML `<bdo>` tag is used to override the current text direction:

>`<bdo dir="rtl">This text will be written from right to left</bdo>`

## HTML Comment Tag
* You can add comments to your HTML source by using the following syntax:
* __Note:__ Comments are not displayed by the browser, but they can help document your HTML source code.
>`<!-- Write your comments here -->`
>`<!-- <p>This is another paragraph </p> -->`

## HTML Links - Hyperlinks
* HTML links are hyperlinks.

* You can click on a link and jump to another document.

*When you move the mouse over a link, the mouse arrow will turn into a little hand(cursor:pointer).

* __Note:__ A link does not have to be text. A link can be an image or any other HTML element!

## HTML Links - Syntax
* The HTML `<a>` tag defines a hyperlink. It has the following syntax:

>`<a href="url">link text</a>`
* The most important attribute of the `<a>` element is the href attribute, which indicates the link's destination.

* The link text is the part that will be visible to the reader.

>`<a href="https://www.google.com/">Visit google.com!</a>`

* By default, links will appear as follows in all browsers:

    * An unvisited link is underlined and blue
    * A visited link is underlined and purple
    * An active link is underlined and red
* __Tip:__ Links can of course be styled with CSS, to get another look!

## HTML Links - The target Attribute
* By default, the linked page will be displayed in the current browser window. To change this, you must specify another target for the link.

* The target attribute specifies where to open the linked document.

* The target attribute can have one of the following values:

    * ___self-__ Default. Opens the document in the same window/tab as it was clicked
    * ___blank-__ Opens the document in a new window or tab
    * ___parent-__ Opens the document in the parent frame
* ___top-__ Opens the document in the full body of the window


>`<a href="https://www.google.com/" target="_blank">Visit Google!</a>`

## HTML Links - Use an Image as a Link
* To use an image as a link, just put the `<img>` tag inside the `<a>` tag:

>`<a href="default.asp"><img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;"></a>`

## Link to an Email Address
* Use mailto: inside the href attribute to create a link that opens the user's email program (to let them send a new email):

>`<a href="mailto:someone@example.com">Send email</a>`

## Button as a Link

* To use an HTML button as a link, you have to add some JavaScript code.

* JavaScript allows you to specify what happens at certain events, such as a click of a button:

>`<button onclick="document.location='default.asp'">HTML Tutorial</button>`
* __Tip:__ Learn more about JavaScript in our JavaScript Tutorial.

## Link Titles
* The title attribute specifies extra information about an element. The information is most often shown as a tooltip text when the mouse moves over the element.

>`<a href="https://www.w3schools.com/html/" title="Go to W3Schools HTML section">Visit our HTML Tutorial</a>`

## Create a Bookmark in HTML
* Bookmarks can be useful if a web page is very long.

* To create a bookmark - first create the bookmark, then add a link to it.

* When the link is clicked, the page will scroll down or up to the location with the bookmark.

* First, use the id attribute to create a bookmark:

>`<h2 id="C4">Chapter 4</h2>`

* Then, add a link to the bookmark ("Jump to Chapter 4"), from within the same page:

>`<a href="#C4">Jump to Chapter 4</a>`

* You can also add a link to a bookmark on another page:

>`<a href="html_demo.html#C4">Jump to Chapter 4</a>`

## HTML Images
* Images can improve the design and the appearance of a web page.

## HTML Images Syntax
* The HTML `<img>` tag is used to embed an image in a web page.

* Images are not technically inserted into a web page; images are linked to web pages. The `<img>` tag creates a holding space for the referenced image.

* The `<img>` tag is empty, it contains attributes only, and does not have a closing tag.

* The `<img>` tag has two required attributes:

* `src` - Specifies the path to the image
* `alt` - Specifies an alternate text for the image
Syntax
>`<img src="url" alt="alternatetext">`

## The src Attribute
* The required src attribute specifies the path (URL) to the image.

* __Note:__ When a web page loads, it is the browser, at that moment, that gets the image from a web server and inserts it into the page. Therefore, make sure that the image actually stays in the same spot in relation to the web page, otherwise your visitors will get a broken link icon. The broken link icon and the alt text are shown if the browser cannot find the image.

Example
>`<img src="rose.jpg" alt="Flower">`

## The alt Attribute
* The required alt attribute provides an alternate text for an image, if the user for some reason cannot view it (because of slow connection, an error in the src attribute, or if the user uses a screen reader).

* The value of the alt attribute should describe the image:

>`<img src="carrot.jpg" alt="a vegetable">`
* If a browser cannot find an image, it will display the value of the alt attribute:

## Image Size - Width and Height
* You can use the style attribute to specify the width and height of an image.

>`<img src="img_baby.jpg" alt="kid in a jacket" style="width:500px;height:600px;">`

* Alternatively, you can use the width and height attributes:

>`<img src="img_boy.jpg" alt="Boy in a jacket" width="500" height="600">`
* The width and height attributes always define the width and height of the image in pixels.

* __Note:__ Always specify the width and height of an image. If width and height are not specified, the web page might flicker while the image loads.

## Images in Another Folder
* If you have your images in a sub-folder, you must include the folder name in the src attribute:

>`<img src="/images/html.jpeg" alt="HTML5 Icon" style="width:179px;height:179px;">`

## Images on Another Server/Website
* Some web sites point to an image on another server.

* To point to an image on another server, you must specify an absolute (full) URL in the src attribute:

>`<img src="https://www.google.com/images/html5.jpg" alt="HTML Logo">`
* **Notes on external images:** External images might be under copyright. If you do not get permission to use it, you may be in violation of copyright laws. In addition, you cannot control external images; they can suddenly be removed or changed.

## Animated Images
* HTML allows animated GIFs:

>`<img src="programming.gif" alt="Computer Man" style="width:48px;height:48px;">`

## Image Floating
* Use the CSS float property to let the image float to the right or to the left of a text:

>`<p><img src="smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">The image will float to the right of the text.</p>`

>`<p><img src="smiley.gif" alt="Smiley face" style="float:left;width:42px;height:42px;">The image will float to the left of the text.</p>`
