# 11c HTML Field Types

## References

* Chapter 7 of the textbook
* [https://www.w3schools.com/html/html_form_input_types.asp](https://www.w3schools.com/html/html_form_input_types.asp)

## Custom field types in general

If the user is on an old browser, most of the custom field types revert to ```type="text"```.

One problem with these new fields is that different browsers render them differently on different platforms.

## Number type

The number type only allows numeric input.

```html
<p>Age: <input type="number" name="number"></p>
```

It is also possible to incorporate a minimum and maximum value with the ```min`` and ```max``` attribute. The min and max values are inclusive.  That is, if min="1" then you may enter 1 as a valid choice.


```html
<p>Age: <input type="number" min="0" max="115" name="number"></p>
```

## Date type

The date input type allows a date to be input.  

Most browsers display some chooser for the date based on the location of computer.  In the US it tends to be mm/dd/yyyy, but in Europe it will tend to be in a format like dd,mm,yyyy.

```html
<p>Birthday: <input type="date" name="birthday"></p>
```

### Min and Max attributes with date

The min and max attributes may be used with dates.  

The problem is that different areas of the world do use different date formats.  The browser can get away with local formats, but there is no way for the browser to determine what format the developer was using when they wrote the min or max date.  Therefore the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format is required.

```html
<p>Desired date (must be before November 21): <input type="date" min="2019-11-12" max="2019-11-21"></p>
```

## Button

The button type is similar to a submit button, but the &lt;button> control, but it does not submit the form.  There is usually a JavaScript onclick action that does something.

```html
<input type="button" onclick="alert('You clicked me!')" value="Click Me!">
```

## email and url types

These are fairly straightforward.

```html
<p>Email: <input type="email"></p>
<p>URL: <input type="url"></p>
```

## There are several other types.

You may look these up as you need them.  See [https://www.w3schools.com/html/html_form_input_types.asp](https://www.w3schools.com/html/html_form_input_types.asp)