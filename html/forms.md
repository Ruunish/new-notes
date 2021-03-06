
##  HTML  Forms:-
An HTML form is used to collect user input. The user input is most often sent to a server for processing.
Example:-
```
<!DOCTYPE html>
<html>
<body>
<h2>HTML Forms</h2>
firstname:<input type="text" name="fname" value="john"><br>
lastname:<input type="text" name="lname" value="doe"><br>
<button>submit</button>
</body>
</html>
```
##  HTML  Form Attributes:-
### The Action Attribute:
The action  attribute defines the action to be performed when the form is submitted.
Usually, the form data is sent to a file on the server when the user clicks on the submit button.
Example:-
```
<!DOCTYPE html>
<html>
<body>
<h2>HTML Forms</h2>
<form action="new.php">
firstname:<input type="text" name="fname" value="john"><br>
lastname:<input type="text" name="lname" value="doe"><br>
<input type="submit" value="submit">
</body>
</html>
```
### The Target Attribute:
The target attribute specifies where to display the response that is received after submitting the form. 
The `target` attribute can have one of the following values:

Value                                           Description
_blank     :                                        The response is displayed in a new window or tab
   _self        :                                     The response is displayed in the current window
_parent   :                                       The response is displayed in the parent frame                                      
_top    :                                           The response is displayed in the full body of the window
_framename_:                            The response is displayed in a named iframe
Example:-
```
<!DOCTYPE html>
<html>
<body>
<h2>HTML Forms</h2>
<form action="new.php" target="_blank">
firstname:<input type="text" name="fname" value="john"><br>
lastname:<input type="text" name="lname" value="doe"><br>
<input type="submit" value="submit">
</body>
</html>
```
### The Method Attribute:-
-The  `method`  attribute specifies the HTTP method to be used when submitting the form       data.
-The form-data can be sent as URL variables (with  `method="get"`) or as HTTP post  (with  `method="post"`).
-The default HTTP method when submitting form data is GET.
-Example for GET method:-
```
<!DOCTYPE html>
<html>
<body>
<h2>HTML Forms</h2>
<form action="new.php" target="_blank" method="get">
firstname:<input type="text" name="fname" value="john"><br>
lastname:<input type="text" name="lname" value="doe"><br>
<input type="submit" value="submit">
</body>
</html>
```
-Example for POST method:-
```
<!DOCTYPE html>
<html>
<body>
<h2>HTML Forms</h2>
<form action="new.php" target="_blank" method="Post">
firstname:<input type="text" name="fname" value="john"><br>
lastname:<input type="text" name="lname" value="doe"><br>
<input type="submit" value="submit">
</body>
</html>
```
## HTML Input Types:-

Here are the different input types you can use in HTML:

-   `<input type="button">`
-   `<input type="checkbox">`
-   `<input type="color">`
-   `<input type="date">`
-   `<input type="datetime-local">`
-   `<input type="email">`
-   `<input type="file">`
-   `<input type="hidden">`
-   `<input type="image">`
-   `<input type="month">`
-   `<input type="number">`
-   `<input type="password">`
-   `<input type="radio">`
-   `<input type="range">`
-   `<input type="reset">`
-   `<input type="search">`
-   `<input type="submit">`
-   `<input type="tel">`
-   `<input type="text">`
-   `<input type="time">`
-   `<input type="url">`
-   `<input type="week">`


# HTML  Input Attributes:-
### The value Attribute:-
The input  `value`  attribute specifies an initial value for an input field:
Example:
```
<!DOCTYPE html>
<html>
<body>
<h2>HTML Forms</h2>
<form action="new.php" target="_blank">
firstname:<input type="text" name="fname" value="john"><br>
lastname:<input type="text" name="lname" value="doe"><br>
<input type="submit" value="submit">
</body>
</html>
```
## The readonly Attribute

-The input  `readonly`  attribute specifies that an input field is read-only.
-A read-only input field cannot be modified (however, a user can tab to it, highlight it, and copy the text from it).
-The value of a read-only input field will be sent when submitting the form!
Example:-
```
<!DOCTYPE html>
<html>
<body>
<h2>HTML Forms</h2>
<form action="new.php" target="_blank">
firstname:<input type="text" name="fname" value="john" readonly><br>
lastname:<input type="text" name="lname" value="doe" readonly><br>
<input type="submit" value="submit">
</body>
</html>
```
### The disabled Attribute:-
-The input  `disabled`  attribute specifies that an input field should be disabled.
-A disabled input field is unusable and un-clickable.
-The value of a disabled input field will not be sent when submitting the form!
Example:-
```
<!DOCTYPE html>
<html>
<body>
<h2>HTML Forms</h2>
<form action="new.php" target="_blank">
firstname:<input type="text" name="fname" value="john" disabled><br>
lastname:<input type="text" name="lname" value="doe" disabled><br>
<input type="submit" value="submit">
</body>
</html>
```
### The size Attribute:-

-The input  `size`  attribute specifies the visible width, in characters, of an input field.
-The default value for  `size`  is 20.
-**Note:**  The  `size`  attribute works with the following input types: text, search, tel, url, email, and password.
Example:-
```
<!DOCTYPE html>
<html>
<body>
<h2>HTML Forms</h2>
<form action="new.php" target="_blank">
firstname:<input type="text" name="fname" size="50"><br>
lastname:<input type="text" name="lname" size="5"><br>
<input type="submit" value="submit">
</body>
</html>
```
### The maxlength Attribute:-

-The input  `maxlength`  attribute specifies the maximum number of characters allowed in an input field.
-**Note:**  When a  `maxlength`  is set, the input field will not accept more than the specified number of characters. However, this attribute does not provide any feedback. So, if you want to alert the user, you must write JavaScript code.
### The multiple Attribute

-The input  `multiple`  attribute specifies that the user is allowed to enter more than one value in an input field.
-The  `multiple`  attribute works with the following input types: email, and file.
Example:-
```
<!DOCTYPE html>
<html>
<body>
<h2>HTML Forms</h2>
<form action="new.php">
	file:<input type="file" name="files" multiple><br>
	<input type="submit" value="upload">
</body>
</html>
```
### The required Attribute:-

-The input  `required`  attribute specifies that an input field must be filled out before submitting the form.
-The  `required`  attribute works with the following input types: text, search, url, tel, email, password, date pickers, number, checkbox, radio, and file.
```
<!DOCTYPE html>
<html>
<body>
<h2>HTML Forms</h2>
<form action="new.php">
	username:<input type="text" name="username" required><br>
	<input type="submit" value="submit">
</body>
</html>
```
### The autofocus Attribute

The input  `autofocus`  attribute specifies that an input field should automatically get focus when the page loads.
Example:-
```
<!DOCTYPE html>
<html>
<body>
<h2>HTML Forms</h2>
<form action="new.php" target="_blank">
firstname:<input type="text" name="fname" autofocus><br>
lastname:<input type="text" name="lname" maxleng="5"><br>
<input type="submit" value="submit">
</body>
</html>
```
### The list Attribute

The input  `list`  attribute refers to a  `<datalist>`  element that contains pre-defined options for an <input> element.
Example:-
```
<!DOCTYPE html>
<html>
<body>
<h2>HTML Forms</h2>
<form action="new.php" target="_blank">
 <input list="schools" name="school">
  <datalist id="schools">
    <option value=" mei">
    <option value="met">
    
  </datalist>
  <input type="submit" value="Submit">
</form>
</body>
</html>
```
