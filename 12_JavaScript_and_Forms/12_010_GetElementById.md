# 12.010 Get Element By ID

The most common method of doing output in JavaScript is to change DOM. In other words, we grab an element on the page and then change its content. This lets us change many things about the item, including the text, the attributes, and style. We can also change its visibility.

## The key function `document.getElementById()`

- Note the "document." Document is an object. The .getElementById() function is part of the Document object.
- Watch out for the capitalization.
  - This is called "camelCase"It is a common programming style when an id contains more than one word
  - The I in id is capitalized, but not the d. This conforms to camelCase style. Consistency is important!

* document.getElementById returns an _Object_.
  - The object is an "Element." There are other functions that also return elements.
  - Most of the Element objects are data fields rather than methods.
  - JavaScript Elements generally conform to HTML elements.
  - See [https://www.w3schools.com/jsref/dom_obj_all.asp](https://www.w3schools.com/jsref/dom_obj_all.asp) for a list of the data fields and functions.
    - In the list, notice that functions always have (). Data fields do not.
    - For the functions, look at the return type.
    - The value in the fields may be changed with JavaScript by using the = to apply a new value.

## The `innerText` property

The innerText is the text that is between the opening and closing tags.

## Replacing the inner text of an element

Given the following HTML,

```html
<p id="name">Unknown</p>
```

The following JavaScript would change "Unknown" so that it now displays "Max Griffon"

```javascript
let nameElement = document.getElementById("name");
nameElement.innerText = "Max Griffon";
```

One limitation on innerText is that it cannot contain any embedded HTML code.

To use text that contains HTML tags,
use `innerHTML` instead of `innerText`

```javascript
let nameElement = document.getElementById("name");
nameElement.innerHTML = "Max <i>the</i> Griffon";
```

## Changing attributes

Attributes may be changed in a manner similar to innerText and innerHTML. Simply name the attribute and give a value for the property.

```javascript
   let linkTag = document.getElementById("sports")
   let linkTag.href="https://gogriffons.com";
```

## Adding Classes

Note that changing the class with a simple assignment would do away with any existing classes associated with the element. This is especially significant when working with Bootstrap. Classes may have many classes, and you don'twant to destroy them.  

The function `addClass()` comes to the rescue.
