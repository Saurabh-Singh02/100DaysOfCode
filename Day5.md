## HTML Favicon
* A favicon is a small image displayed next to the page title in the browser tab.

# How To Add a Favicon in HTML
* You can use any image you like as your favicon. You can also create your own favicon on sites like https://www.favicon.cc.

* __Tip:__ A favicon is a small image, so it should be a simple image with high contrast.

* A favicon image is displayed to the left of the page title in the browser tab, like this:


![favicon](https://github.com/Saurabh-Singh02/100DaysOfCode/assets/122091208/0174ebf9-c834-4914-9aee-ed4df9673e4e)

* To add a favicon to your website, either save your favicon image to the root directory of your webserver, or create a folder in the root directory called images, and save your favicon image in this folder. A common name for a favicon image is "favicon.ico".

* Next, add a `<link>` element to your "index.html" file, after the `<title>` element, like this:

>`<link rel="icon" type="image/x-icon" href="/images/favicon.ico">`

```
<!DOCTYPE html>
<html>
<head>
  <title>My Page Title</title>
  <link rel="icon" type="image/x-icon" href="/images/favicon.ico">
</head>
<body>
<h1>This is a Heading</h1>
<p>This is a paragraph.</p>
</body>
</html>
```
* Now, save the "index.html" file and reload it in your browser. Your browser tab should now display your favicon image to the left of the page title.

## Favicon File Format Support
* The following table shows the file format support for a favicon image:

|Browser |ICO|PNG|GIF|JPEG|SVG|
|--------|---|---|---|----|---|
|Edge	 |Yes|Yes|Yes| Yes|Yes|
|Chrome	 |Yes|Yes|Yes| Yes|Yes|
|Firefox |Yes|Yes|Yes| Yes|Yes|
|Opera	 |Yes|Yes|Yes| Yes|Yes|
|Safari	 |Yes|Yes|Yes| Yes|Yes|

* `<link>`	Defines the relationship between a document and an external resource
For a complete list of all available HTML tags, visit our HTML Tag Reference.

## HTML Tables
* HTML tables allow web developers to arrange data into rows and columns.

|continent|country|capital|
|---------|-------|-------|
|Asia     |India  |New Delhi|
|Africa     |Egypt  |Cairo|
|Europe     |Ukrain  |Kev|
```
<table>
  <tr>
    <th>Company</th>
    <th>Contact</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>Alfreds Futterkiste</td>
    <td>Maria Anders</td>
    <td>Germany</td>
  </tr>
  <tr>
    <td>Centro comercial Moctezuma</td>
    <td>Francisco Chang</td>
    <td>Mexico</td>
  </tr>
</table>
```
## Table Cells
* Each table cell is defined by a `<td>` and a `</td>` tag.

* `td` stands for table data.

* Everything between `<td>` and `</td>` are the content of the table cell.
```
<table>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
</table>
```
* __Note:__ A table cell can contain all sorts of HTML elements: text, images, lists, links, other tables, etc.

## Table Rows
* Each table row starts with a `<tr>` and ends with a `</tr>` tag.

* `tr` stands for table row.

```
<table>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
  <tr>
    <td>16</td>
    <td>14</td>
    <td>10</td>
  </tr>
</table>
```
* You can have as many rows as you like in a table; just make sure that the number of cells are the same in each row.

* __Note:__ There are times when a row can have less or more cells than another. You will learn about that in a later chapter.

## Table Headers
* Sometimes you want your cells to be table header cells. In those cases use the `<th>` tag instead of the `<td>` tag:

* `th` stands for table header.

* Let the first row be table header cells:
```
<table>
  <tr>
    <th>Person 1</th>
    <th>Person 2</th>
    <th>Person 3</th>
  </tr>
  <tr>
    <td>Emil</td>
    <td>Tobias</td>
    <td>Linus</td>
  </tr>
  <tr>
    <td>16</td>
    <td>14</td>
    <td>10</td>
  </tr>
</table>
```
* By default, the text in `<th>` elements are bold and centered, but you can change that with CSS.

## HTML Table Colspan & Rowspan
* HTML tables can have cells that span over multiple rows and/or columns.

![colspan   rowspan](https://github.com/Saurabh-Singh02/100DaysOfCode/assets/122091208/21917f59-35d3-4c2d-aad2-64be3bc78072)


## HTML Table - Colspan
* To make a cell span over multiple columns, use the colspan attribute:

>`<th colspan="2">Name</th>`

```
<table>
  <tr>
    <th colspan="2">Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>43</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>57</td>
  </tr>
</table>
```
* __Note:__ The value of the colspan attribute represents the number of columns to span.

## HTML Table - Rowspan
* To make a cell span over multiple rows, use the rowspan attribute:

>`<th rowspan="2">Phone</th>`
```
<table>
  <tr>
    <th>Name</th>
    <td>Jill</td>
  </tr>
  <tr>
    <th rowspan="2">Phone</th>
    <td>555-1234</td>
  </tr>
  <tr>
    <td>555-8745</td>
</tr>
</table>
```
* __Note:__ The value of the rowspan attribute represents the number of rows to span.

## HTML Lists
* HTML lists allow web developers to group a set of related items in lists.


An unordered HTML list:

* Item
* Item
* Item
* Item

An ordered HTML list:

1. First item
2. Second item
3. Third item
4. Fourth item

**Unordered HTML List**
* An unordered list starts with the `<ul>` tag. Each list item starts with the `<li>` tag.

* The list items will be marked with bullets (small black circles) by default:

```
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```
|Value|	Description|
|-----|------------|
|disc |	Sets the list item marker to a bullet (default)|
|circle|	Sets the list item marker to a circle|
|square	|Sets the list item marker to a square|
|none	|The list items will not be marked|

**Nested HTML Lists**
* Lists can be nested (list inside list):

```
<ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea</li>
    </ul>
  </li>
  <li>Milk</li>
</ul>
```
* Tea
    * Black Tea
    * Green Tea

**Ordered HTML List**
* An ordered list starts with the `<ol>` tag. Each list item starts with the `<li>` tag.

* The list items will be marked with numbers by default:

```
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```
**Ordered HTML List - The Type Attribute**
* The type attribute of the `<ol>` tag, defines the type of the list item marker:
>`<ol type="1">`

|Type|	Description|
|----|-------------|
|type="1"|	The list items will be numbered with numbers (default)|
|type="A"|	The list items will be numbered with uppercase letters|
|type="a"|	The list items will be numbered with lowercase letters|
|type="I"|	The list items will be numbered with uppercase roman numbers|
|type="i"|	The list items will be numbered with lowercase roman numbers|

**Control List Counting**
* By default, an ordered list will start counting from 1. If you want to start counting from a specified number, you can use the start attribute:
>`<ol start="50">`
```
<ol start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

**HTML Description Lists**
* HTML also supports description lists.

* A description list is a list of terms, with a description of each term.

* The `<dl>` tag defines the description list, the `<dt>` tag defines the term (name), and the `<dd>` tag describes each term:

```
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
```
