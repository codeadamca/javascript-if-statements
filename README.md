# A Basic Introduction to JavaScript and If Statements

JavaScript `if` statements allow code to make decisions. A typical `if` statement has the following structure:

```javascript
if(variable == "value")
{
  // Code to execute when condition is true
}
```

An `if` statement causes the block of code between the open `{` and close `}` to only be executed if the condition between the open `(` and close `)` is true. When writing a condition, the following operators can be used:

<table>
<tr><th>Operator</th><th>Description</th></tr>
<tr><td>==</td><td>Equal to</td></tr>
<tr><td>!=</td><td>Not equal to</td></tr>
<tr><td>&gt;</td><td>Greater than</td></tr>
<tr><td>&lt;</td><td>Less than</td></tr>
<tr><td>&gt;=</td><td>Greater than or equal to</td></tr>
<tr><td>&lt;=</td><td>Less than or equal to</td></tr>
</table>

## Validation

JavaScript `if` statements are commonly used when validating a form. Create a new `HTML` document and add the following code:

```html
<!doctype html>
<html>
<head>
    <title>JavaScript If Statements</title>
</head>
<body>

    <h1>JavaScript If Statements</h1>

    <p>Enter some text:</p>

    <input type="text" id="text">

    <br>

    <button id="check">Check</button>

</body>
</html>
```

When the button is pressed, we will display a message indicating if the textbox has a value or is blank. We will achieve this by using an `if` statement followed by an `else` statement. The block of code associated to the `else` is executed if the condition of the `if` statement is false:

```javascript
if(variable == "value")
{
  // Code to execute when condition is true
}
else
{
  // Code to execute when condition is false
}
```

Add a `script` tag below the button in the new doucument. Add the following JavaScript to check the textbox and display a message:

```javascript
  var button = document.getElementById("check");

  button.addEventListener("click", function(){

      var textbox = document.getElementById("text");

      if(textbox.value == "")
      {
          alert("The textbox is empty!");
      }
      else
      {
          alert("The textbox has a value");
      }

  });
```

## Try It Out

Create a new HTML document, add the standard HTML tags, and a title:

```html
<!doctype html>
<html>
<head>
    <title>JavaScript Greeting</title>
</head>
<body>

    <h1>JavaScript Greeting</h1>

</body>
</html>
```

After the title add a `script` tag and the following JavaScript:

```javascript
var now = new Date();

var day = now.getDay();
var hour = now.getHours();

document.write("<p>The current day is " + day + ".</p>");
document.write("<p>The current hour is " + hour + ".</p>");
```

This code creates a date object and uses the `getDay()` and `getHours()` to extract the day of the week (0 for Sunday and 6 for Saturday) and the hour of the day (in a 24 hours format). 

After the previous JavaScript add an `if` statement to display a greeting based on the time of day and day of week:

<table>
<tr><th>Condition</th><th>Message</th></tr>
<tr><td>Monday</td><td>Does someone have a case of the Mondays!</td></tr>
<tr><td>Friday afternoon</td><td>TGIF!</td></tr>
<tr><td>Weekend</td><td>Have a great weekend!</td></tr>
<tr><td>Other mornings</td><td>Good morning!</td></tr>
<tr><td>Other afternoons</td><td>Good afternoon!</td></tr>
</table>

> Full tutorial URL:  
> https://codeadam.ca/learning/javascript-if-statements.html

***

## Repo Resources

* [Visual Studio Code](https://code.visualstudio.com/)
* [W3Schools - JavaScript](https://www.w3schools.com/js/)

<a href="https://codeadam.ca">
<img src="https://codeadam.ca/images/code-block.png" width="100">
</a>

