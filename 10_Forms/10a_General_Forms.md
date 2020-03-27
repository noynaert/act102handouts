# 10a General Forms

## References

* [W3schools on forms](https://www.w3schools.com/html/html_forms.asp)
* Textbook, chapter 7

## Uses of forms

Forms allow the user to interact with a website. Users may enter data, click buttons, or use otehr controls.

The form can do different things with the user interaction:

1. Send data to another web site for processing
2. Use JavaScript on the same page to manipulate data entered by the user
3. Some combination of the above.

## Form using GET method to remote site

* ***Action*** attribute: The &lt;form> tag takes an action attribute.  The action is usually a url of a page that processes data and shows a result.  In some cases the action may be the same page.
* ***Method*** attribute: The &lt;form> tag takes a method attribute.  There are 6 possible methods, but we will only consider "GET" and "POST" methods.  

```html
<form method="GET" action="https://webservices.missouriwestern.edu/users/noynaert/act102/api/generic.php">

</form>
```

### Controls

There are several controls that may go in a form.  HTML5 introduced quite a few more, but most are just variations on the old types.

Controls go inside a &lt;form> tag, although many of the controls can appear outside a form tag for special purposes.

Most controls do not have any explanatory text.  Therefore they usually go in a &lt;label> tag with the text.  We may use &lt;p>, &lt;br> tags, or tables to organize the table visually.

### &lt;input type="text" name="age">

This is for a single line of text input.  The name is important.  It should be descriptive of the contents of the field. As usual keep it simple, meaningful, and use lower case.  Make it a single word.

There are other fields we could enter.  For example, the value attribute gives an initial set of text to the field.

Be careful using old websites about input fields.  Things like the "size" tag in the input field should no longer be used.

### &lt;input type="submit">

This is one way to submit the contents of a form.  You may give it a name, but do not have to.  You may also change the contents of the button by specifying a value.

```html
<h1>Forms</h1>
    <h2>Text input and submit button</h2>
    <form method="GET" action="https://webservices.missouriwestern.edu/users/noynaert/act102/api/generic.php">
        <p>
          <label>Age:</label>
          <input type="text" name="age" value="18"> 
        </p>
        <p>
          <label>Height:</label> <input type="text" name="feet">ft. <input type="text" name="inches">in.
        </p>
        <input type="submit">
      </form>
```
![Example of Text Input in the browser](exampleCode/images/01TextAndSubmit.png)


#### Text and &lt;label> tags

The &lt;input> tag does not have any type of label associated with it.  But users almost certainly need a label. Text can be just inserted within the form.  It is also possible to use div, p, table, and br tags to control layout.

In later versions of html there is a &lt;label>...&lt;/label> tag.  It is a good idea to use label tags with input fields and any other field that does not have its own text and labels built in.

#### For advanced users

[Here is a nice tutorial on animated input boxes](https://www.youtube.com/watch?v=IxRJ8vplzAo).  It is optional, and only for people that are bored or want some extra material.

## Methods -- GET and POST

The http protocol has several methods for sending data from the client to the server:

* GET
* POST
* PUT
* HEAD
* DELETE
* PATCH
* OPTIONS

However, in this course we will only be concerned with GET and POST, and we will mainly use GET.

### GET Method

* Get is used to retrieve information from a server
* Get data is sent in the URL itself
* ? is used to separate the base URL from the fields. 
* & is used between fields
* The format of each field is `name=value`
* If there are blank spaces, the values must be "url encoded"

```
https://catfact.ninja/facts?limit=5
```
* The web site itself is `catfact.ninja/facts`
* ? indicates the start of data
* `limit` is the number of facts requested
* `5` facts are being requested
* Try putting the url in your browser.  Try to get different numbers

```
https://webservices.missouriwestern.edu/users/noynaert/act102/api/generic.php?age=18&feet=5&inches=11
```
* The web site itself is https://webservices.missouriwestern.edu/users/noynaert/act102/api/generic.php
* There are three fields.  Age is 18, feet is 5, and inches are 11.  Try some different values.  Also, try adding a weight field with a value of 150.

```
https://webservices.missouriwestern.edu/users/noynaert/act102/api/generic.php?first="Frank"&last=Von%20Peure%2C%20Sr.
```

Text input gets tricky if you type in blanks or most special characters. In the above URL look at how the blank and comma were encoded.

Browsers automatically do URL encoding as necessary when blanks or special characters are parts of input fields on a form.  You can explore encoding on your own at [https://www.urlencoder.io/](https://www.urlencoder.io/)

**Advantages of GET method**

URLs may be copy/pasted, bookmarked, and cached

**Disadvantages of GET method**

* URL total length must be under 2048 characters
* URL encoding only works with ASCII characters (not unicode)
* Not good for sensitive information like passwords

### POST method

Technically the POST method is supposed to be used for "posting" new information to a database or other data repository.  However, it is often used as an alternative to the GET method.

The POST method passes data in headers "behind the scene."  This means the data being passed is not available in the URL.  The data in POST may be encrypted for security.

* POST method does not limit the length
* POST data cannot be cached
* POST data is not stored in the browser history

## APIs

API means "Application Programming Interface."  There are a couple of different meanings to API, but in this class an API means a web site that processes data from a GET, PUT, or other method and returns some data.

APIs can return data in a variety of formats.  The most common are

* JSON (The most common form currently.  CatFacts uses this format)
* XML (related to html, but with more flexible tags)
* plain text
* .csv format that may be loaded into Excel
* .html format as a webpage
  