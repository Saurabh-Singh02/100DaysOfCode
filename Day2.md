## How to use HTML? 
* Open notepad or any text editor (like atom, sublime, vscode, etc)
* Write your HTML code.
* Save the HTML page.
    * Name the file "index.html" and set the encoding to UTF-8 (which is the preferred encoding for HTML files).
    * You can use either .htm or .html as file extension. There is no difference; it is up to you.
* Open the saved HTML file in your favorite browser (double click on the file, or right-click - and choose "Open with"). 
## HTML Document
* HTML is not case sensitive.
* The HTML standard doesn't require lowercase attribute names.

* The title attribute (and all other attributes) can be written with uppercase or lowercase like title or TITLE.

* However, W3C recommends lowercase attributes in HTML, and demands lowercase attributes for stricter document types like XHTML.
* All HTML documents must start with a document type declaration: `<!DOCTYPE html>`.   
* The HTML document itself begins with `<html>` and ends with `</html>`.
* The visible part of the HTML document is between `<body>` and `</body>`.
```
<!DOCTYPE html>
<html>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```
## The <!DOCTYPE> Declaration
* The `<!DOCTYPE>` declaration represents the document type (for HTML5), and helps browsers to display web pages correctly.
* It must only appear once, at the top of the page (before any HTML tags).
* The <!DOCTYPE> declaration is not case sensitive.
* The <!DOCTYPE> declaration for HTML5 is:
> `<!DOCTYPE html>`
## HTML title tag
* `<tittle>` tag define the title of your webpage.
* This title appers inside the tab of the browser when you open your webpage.
>`<title> my first website</title>`
## HTML Headings
* HTML headings are defined with the `<h1>` to `<h6>` tags.

* `<h1>` defines the most important heading. `<h6>` defines the least important heading: 
>`<h1>`heading`</h1>`
## HTML Paragraphs
* HTML paragraphs are defined with the `<p>` tag:
>`<p>`this is a paragraph`</p>`
## The style Attribute
* The style attribute is used to add styles to an element, such as color, font, size, and more.

>`<p style="color:red;">This is a red paragraph.</p>`
## HTML Links
* HTML links are defined with the `<a>` tag:
>`<a href="">`link`</a>`
* The link's destination is specified in the `href` attribute. 

* Attributes are used to provide additional information about HTML elements.
## HTML Images
* HTML images are defined with the `<img>` tag.

* The source file `(src)`, alternative text `(alt)`, `width`, and `height` are provided as attributes:
>`<img src="w3schools.jpg" alt="W3Schools.com" width="104" height="142">`
## The src Attribute
<img src="xyz.jpg" alt="xyz.com" width="104" height="142">

The `<img>` tag is used to embed an image in an HTML page. The `src` attribute specifies the path to the image to be displayed:

>`<img src="img_girl.jpg">`
## The width and height Attributes
* The `<img>` tag should also contain the width and height attributes, which specify the width and height of the image (in pixels):

>`<img src="img_girl.jpg" width="500" height="600">`
<img src="img_girl.jpg" width="400" height="200">
## How to View HTML Source
1. __View HTML Source Code:__
    * Right-click in an HTML page and select "View Page Source" (in Chrome) or "View Source" (in Edge), or similar in other browsers. This will open a window containing the HTML source code of the page.

2. __Inspect an HTML Element:__
    * Right-click on an element (or a blank area), and choose "Inspect" or "Inspect Element" to see what elements are made up of (you will see both the HTML and the CSS). You can also edit the HTML or CSS on-the-fly in the Elements or Styles panel that opens.

* There are two ways to specify the URL in the src attribute:

    1. __Absolute URL__ - Links to an external image that is hosted on another website. Example: src="https://www.google.com/images/img_girl.jpg".

    * __Notes__: External images might be under copyright. If you do not get permission to use it, you may be in violation of copyright laws. In addition, you cannot control external images; it can suddenly be removed or changed.

    2. __Relative URL__ - Links to an image that is hosted within the website. Here, the URL does not include the domain name. If the URL begins without a slash, it will be relative to the current page. Example: src="img_girl.jpg". If the URL begins with a slash, it will be relative to the domain. Example: src="/images/img_girl.jpg".

    * __Tip:__ It is almost always best to use relative URLs. They will not break if you change domain.


