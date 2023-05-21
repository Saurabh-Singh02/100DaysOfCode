## The HTML `<form>` Elements
* The HTML `<form>` element can contain one or more of the following form elements:
```
<input>
<label>
<select>
<textarea>
<button>
<fieldset>
<legend>
<datalist>
<output>
<option>
<optgroup>
```
## The `<input>` Element
* One of the most used form element is the `<input>` element.

* The `<input>` element can be displayed in several ways, depending on the type attribute.

```
<label for="fname">First name:</label>
<input type="text" id="fname" name="fname">
```

## The `<label>` Element
* The `<label>` element defines a label for several form elements.

* The `<label>` element is useful for screen-reader users, because the screen-reader will read out loud the label when the user focus on the input element.

8 The `<label>` element also help users who have difficulty clicking on very small regions (such as radio buttons or checkboxes) - because when the user clicks the text within the <label> element, it toggles the radio button/checkbox.

* The for attribute of the `<label>` tag should be equal to the id attribute of the `<input>` element to bind them together.

## The `<select>` Element
* The `<select>` element defines a drop-down list:
```
<label for="cars">Choose a car:</label>
<select id="cars" name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```
* The `<option>` elements defines an option that can be selected.

* **By default,** the **first item** in the drop-down list is selected.

* To define a pre-selected option, add the selected attribute to the option:

```
<option value="fiat" selected>Fiat</option>
```
**Visible Values:**
* Use the size attribute to specify the number of visible values:

```
<label for="cars">Choose a car:</label>
<select id="cars" name="cars" size="3">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```
**Allow Multiple Selections:**
* Use the multiple attribute to allow the user to select more than one value:

```
<label for="cars">Choose a car:</label>
<select id="cars" name="cars" size="4" multiple>
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```

## The `<textarea>` Element
* The `<textarea>` element defines a multi-line input field (a text area):
```
<textarea name="message" rows="10" cols="30">
The cat was playing in the garden.
</textarea>
```
* The rows attribute specifies the visible number of lines in a text area.

* The cols attribute specifies the visible width of a text area.



* You can also define the size of the text area by using CSS:
```
<textarea name="message" style="width:200px; height:600px;">
The cat was playing in the garden.
</textarea>
```
## The `<button>` Element
* The `<button>` element defines a clickable button:

`<button type="button" onclick="alert('Hello World!')">Click Me!</button>`

* **Note:** Always specify the type attribute for the button element. Different browsers may use different default types for the button element.

## The `<fieldset>` and `<legend>` Elements
* The  `<fieldset>` element is used to group related data in a form.

* The `<legend>` element defines a caption for the `<fieldset>` element.
```
<form action="/action_page.php">
  <fieldset>
    <legend>Personalia:</legend>
    <label for="fname">First name:</label><br>
    <input type="text" id="fname" name="fname" value="John"><br>
    <label for="lname">Last name:</label><br>
    <input type="text" id="lname" name="lname" value="Doe"><br><br>
    <input type="submit" value="Submit">
  </fieldset>
</form>
```

## The `<datalist>` Element
* The `<datalist>` element specifies a list of pre-defined options for an `<input>` element.

* Users will see a drop-down list of the pre-defined options as they input data.

* The list attribute of the `<input>` element, must refer to the id attribute of the `<datalist>` element.

```
<form action="/action_page.php">
  <input list="browsers">
  <datalist id="browsers">
    <option value="Internet Explorer">
    <option value="Firefox">
    <option value="Chrome">
    <option value="Opera">
    <option value="Safari">
  </datalist>
</form>
```
## The `<output>` Element
* The `<output>` element represents the result of a calculation (like one performed by a script).

* Perform a calculation and show the result in an `<output>` element:
```
<form action="/action_page.php"
  oninput="x.value=parseInt(a.value)+parseInt(b.value)">
  0
  <input type="range"  id="a" name="a" value="50">
  100 +
  <input type="number" id="b" name="b" value="50">
  =
  <output name="x" for="a b"></output>
  <br><br>
  <input type="submit">
</form>
```


## HTML Input Types
* Here are the different input types you can use in HTML:
```
<input type="button">
<input type="checkbox">
<input type="color">
<input type="date">
<input type="datetime-local">
<input type="email">
<input type="file">
<input type="hidden">
<input type="image">
<input type="month">
<input type="number">
<input type="password">
<input type="radio">
<input type="range">
<input type="reset">
<input type="search">
<input type="submit">
<input type="tel">
<input type="text">
<input type="time">
<input type="url">
<input type="week">
```
* **Tip:** The default value of the type attribute is "text".

### Input Type `Text`

* `<input type="text">` defines a single-line text input field:
```
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```

### Input Type `Password`
* `<input type="password">` defines a password field:
```
<form>
  <label for="username">Username:</label><br>
  <input type="text" id="username" name="username"><br>
  <label for="pwd">Password:</label><br>
  <input type="password" id="pwd" name="pwd">
</form>
```

### Input Type `Submit`
* `<input type="submit">` defines a button for submitting form data to a form-handler.

* The form-handler is typically a server page with a script for processing input data.

* The form-handler is specified in the form's action attribute:
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

* If you omit the submit button's value attribute, the button will get a default text:
```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit">
</form>
```
### Input Type `Reset`
* `<input type="reset">` defines a reset button that will reset all form values to their default values:

```
<form action="/action_page.php">
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
  <input type="reset">
</form>
```
 
* If you change the input values and then click the "Reset" button, the form-data will be reset to the default values.

## Input Type `Radio`
`<input type="radio">` defines a radio button.

* Radio buttons let a user select ONLY ONE of a limited number of choices:

```
<p>Choose your favorite Web language:</p>
<form>
  <input type="radio" id="html" name="fav_language" value="HTML">
  <label for="html">HTML</label><br>
  <input type="radio" id="css" name="fav_language" value="CSS">
  <label for="css">CSS</label><br>
  <input type="radio" id="javascript" name="fav_language" value="JavaScript">
  <label for="javascript">JavaScript</label>
</form>
```
### Input Type `Checkbox`
* `<input type="checkbox">` defines a checkbox.

* Checkboxes let a user select ZERO or MORE options of a limited number of choices.
```
<form>
  <input type="checkbox" id="vehicle1" name="vehicle1" value="Bike">
  <label for="vehicle1"> I have a bike</label><br>
  <input type="checkbox" id="vehicle2" name="vehicle2" value="Car">
  <label for="vehicle2"> I have a car</label><br>
  <input type="checkbox" id="vehicle3" name="vehicle3" value="Boat">
  <label for="vehicle3"> I have a boat</label>
</form>
```
### Input Type `Button`
* `<input type="button">` defines a button:

`<input type="button" onclick="alert('Hello World!')" value="Click Me!">`

### Input Type `Color`
* The `<input type="color">` is used for input fields that should contain a color.

* Depending on browser support, a color picker can show up in the input field.

```
<form>
  <label for="favcolor">Select your favorite color:</label>
  <input type="color" id="favcolor" name="favcolor">
</form>
```

### Input Type `Date`
* The `<input type="date">` is used for input fields that should contain a date.

* Depending on browser support, a date picker can show up in the input field.
```
<form>
  <label for="birthday">Birthday:</label>
  <input type="date" id="birthday" name="birthday">
</form>
```
* You can also use the `min` and `max` attributes to add restrictions to dates:
```
<form>
  <label for="datemax">Enter a date before 1980-01-01:</label>
  <input type="date" id="datemax" name="datemax" max="1979-12-31"><br><br>
  <label for="datemin">Enter a date after 2000-01-01:</label>
  <input type="date" id="datemin" name="datemin" min="2000-01-02">
</form>
```
### Input Type `Datetime-local`
* The   <input type="datetime-local">` specifies a date and time input field, with no time zone.

* Depending on browser support, a date picker can show up in the input field.

```
<form>
  <label for="birthdaytime">Birthday (date and time):</label>
  <input type="datetime-local" id="birthdaytime" name="birthdaytime">
</form>
```
### Input Type `Email`
* The `<input type="email">` is used for input fields that should contain an e-mail address.

* Depending on browser support, the e-mail address can be automatically validated when submitted.

* Some smartphones recognize the email type, and add ".com" to the keyboard to match email input.

```
<form>
  <label for="email">Enter your email:</label>
  <input type="email" id="email" name="email">
</form>
```
### Input Type `Image`
* The `<input type="image">` defines an image as a submit button.

* The path to the image is specified in the src attribute.

```
<form>
<input type="image" src="img_submit.gif" alt="Submit" width="48" height="48">
</form>
```
### Input Type `File`
* The `<input type="file">` defines a file-select field and a "Browse" button for file uploads.

```
<form>
  <label for="myfile">Select a file:</label>
  <input type="file" id="myfile" name="myfile">
</form>
```
### Input Type `Hidden`
* The `<input type="hidden">` defines a hidden input field (not visible to a user).

* A hidden field lets web developers include data that cannot be seen or modified by users when a form is submitted.

* A hidden field often stores what database record that needs to be updated when the form is submitted.

* **Note:** While the value is not displayed to the user in the page's content, it is visible (and can be edited) using any browser's developer tools or "View Source" functionality. Do not use hidden inputs as a form of security!

```
<form>
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <input type="hidden" id="custId" name="custId" value="3487">
  <input type="submit" value="Submit">
</form>
```
### Input Type `Month`
* The `<input type="month">` allows the user to select a month and year.

* Depending on browser support, a date picker can show up in the input field.
```
<form>
  <label for="bdaymonth">Birthday (month and year):</label>
  <input type="month" id="bdaymonth" name="bdaymonth">
</form>
```
### Input Type `Number`
The `<input type="number">` defines a numeric input field.

* You can also set restrictions on what numbers are accepted.

* The following example displays a numeric input field, where you can enter a value from 1 to 5:

```
<form>
  <label for="quantity">Quantity (between 1 and 5):</label>
  <input type="number" id="quantity" name="quantity" min="1" max="5">
</form>
```
### Input `Restrictions`
* Here is a list of some common input restrictions:

|Attribute|	Description|
|---------|------------|
|checked|	Specifies that an input field should be pre-selected when the page loads (for type="checkbox" or type="radio")|
|disabled|	Specifies that an input field should be disabled
|max|	Specifies the maximum value for an input field|
|maxlength|	Specifies the maximum number of character for an input field|
|min|	Specifies the minimum value for an input field|
|pattern|	Specifies a regular expression to check the input value against|
|readonly|	Specifies that an input field is read only (cannot be changed)|
|required|	Specifies that an input field is required (must be filled out)|
|size|	Specifies the width (in characters) of an input field|
|step|	Specifies the legal number intervals for an input field|
|value|	Specifies the default value for an input field|

* The following example displays a numeric input field, where you can enter a value from 0 to 100, in steps of 10. The default value is 30:

```
<form>
  <label for="quantity">Quantity:</label>
  <input type="number" id="quantity" name="quantity" min="0" max="100" step="10" value="30">
</form>
```
### Input Type `Range`
* The `<input type="range">` defines a control for entering a number whose exact value is not important (like a slider control). Default range is 0 to 100. However, you can set restrictions on what numbers are accepted with the min, max, and step attributes:

```
<form>
  <label for="vol">Volume (between 0 and 50):</label>
  <input type="range" id="vol" name="vol" min="0" max="50">
</form>
```
### Input Type `Search`
* The `<input type="search">` is used for search fields (a search field behaves like a regular text field).

```
<form>
  <label for="gsearch">Search Google:</label>
  <input type="search" id="gsearch" name="gsearch">
</form>
```
### Input Type `Tel`
* The `<input type="tel">` is used for input fields that should contain a telephone number.

```
<form>
  <label for="phone">Enter your phone number:</label>
  <input type="tel" id="phone" name="phone" pattern="[0-9]{3}-[0-9]{2}-[0-9]{3}">
</form>
```
* Input Type `Time`
* The `<input type="time">` allows the user to select a time (no time zone).

* Depending on browser support, a time picker can show up in the input field.

```
<form>
  <label for="appt">Select a time:</label>
  <input type="time" id="appt" name="appt">
</form>
```
### Input Type `Url`
* The `<input type="url">` is used for input fields that should contain a URL address.

* Depending on browser support, the url field can be automatically validated when submitted.

* Some smartphones recognize the url type, and adds ".com" to the keyboard to match url input.
```
<form>
  <label for="homepage">Add your homepage:</label>
  <input type="url" id="homepage" name="homepage">
</form>
```
### Input Type `Week`
* The `<input type="week">` allows the user to select a week and year.

* Depending on browser support, a date picker can show up in the input field.

```
<form>
  <label for="week">Select a week:</label>
  <input type="week" id="week" name="week">
</form>
```