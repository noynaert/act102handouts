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

Most controls do not have any explanatory text.  Therefore they usually go in a &lt;p> tag with the text

### &lt;input type="text" name="age">

This is for a single line of text input.  The name is important.  It should be descriptive of the contents of the field. As usual keep it simple, meaningful, and use lower case.  Make it a single word.

There are other fields we could enter.  The value attribute gives an initial set of text to the field.

```html
<form method="GET" action="https://webservices.missouriwestern.edu/users/noynaert/act102/api/generic.php">
  <p>
    Age: 
    <input type="text" name="age" value="18"> 
  </p>
  <p>
    Height: <input type="text" name="feet">ft. <input type="text" name="inches">in.
  </p>
  <input type="submit">
</form>
```