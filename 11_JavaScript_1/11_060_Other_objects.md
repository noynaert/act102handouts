# 13f Other Objects

So far we have have used "this" to allow an object to modify itself.

```javascript
<script>
    function mouseOver(me) {
      me.style.color = "blue";
      me.style.backgroundColor = "lightblue";
    }
...
   <h1 onmouseover="mouseOver(this)">Something</h1>
```
## Interacting with other objects

### Getting other elements

The JavaScript function ```document.getElementById("???")``` is one of the most important in JavaScript.  It gets an object that is assigned an Id.

---
#### Why not get Elements By Class?

There are other ways to get elements.  But most of them return more than one result.  This means they have to return an array of elements, and arrays is beyond what we are doing in this course.

If you are comfortable working with arrays, check out [https://www.w3schools.com/js/js_htmldom_elements.asp](https://www.w3schools.com/js/js_htmldom_elements.asp).

---

### Example

The full example is a bit long, so if you want to see or get the code look in the repo at [https://raw.githubusercontent.com/noynaert/ACT102_Notes/master/13_JavaScript/examples/06_buttons.html](https://raw.githubusercontent.com/noynaert/ACT102_Notes/master/13_JavaScript/examples/06_buttons.html) and pick the "Raw" view.

```javascript
  function getKitten(){
    var image;
    image = document.getElementById("pet");
    image.src = "images/kitten.jpg";
    image.alt = "A Kitten";
  }
  ...
  <img src="images/puppy.jpg" alt="A Puppy" id="pet">
  <button onclick="getKitten">Show Kitten</button>
  }
```
## Arithmetic Operators

|Operator|Description|
:-:|---
|+|Addition|
|-|Subtraction|
|*|Multiplication|
|/|Division|

```javascript
console.log(6+4) //prints 10
console.log(6-4) //prints 2
console.log(6*4) //prints 24
console.log(6/4) //prints 1.5
```


For people who know other programming languages, a full set of arithmetic operators is available at [https://www.w3schools.com/js/js_arithmetic.asp](https://www.w3schools.com/js/js_arithmetic.asp)  These extra operators will not be on the final.