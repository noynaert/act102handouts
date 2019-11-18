#13c EventHandlers

## Resources

* [W3Schools Elements](https://www.w3schools.com/jsref/dom_obj_all.asp)
* [W3Schools Event Handlers](https://www.w3schools.com/js/js_events.asp)

## Element Objects

### Elements

HTML Elements are tags like ```<div>```, ```<head>```, or ```<img>```.

### Objects

Objects are something we use in Javascript.  Objects are hard to define, but roughly we will consider it a group of characteristics related to one thing.

JavaScript treats each HTML element as an object.

#### Objects may contain other objects

For HTML objects, the attributes are also objects.  We can specify the sub-objects with a period.

```javascript
console.log(paragraph.style);
console.log(paragraph.style.color);
paragraph.style.color = "green";
```

## Event Handlers

There are hundreds of events that can happen on a web page.

* An element on a page loads
* User moves the mouse
* User pushes or releases a key on the keyboard
* Media starts playing or changes in some way

In JavaScript event handlers are ***attributes*** that begin with "on"  Here are some examples

* onclick
* onmouseover
* onmouseout
* onchange

The event handlers are attributes in HTML.  The values are a JavaScript function.  For now we will use built-in functions, but later we will write our own.  Note we are using single quotes inside double quotes.

```html
<h1 onmouseover="console.log('I am in')">Hello</h1>
<button onclick="console.log(new Date())">Click Me!</button>
<p onmouseover="console.log('In paragraph')" onmouseOut="console.log('Leaving Paragraph')">This is a paragraph</p>
<p><input type="text" onchange="console.log('My value is '+ this.value)"></p>
```

## The importance of ***this***

In object oriented programming "this" refers to the current argument.  It can be passed as an argument to a function.  In this case we are going to use + with a string to concatenate them.

```html
<h1 onmouseover="console.log('I am in ' + this)">Hello</h1>
<p onmouseover="console.log('In paragraph')" onmouseOut="console.log('Leaving Paragraph')">This is a paragraph</p>
```
