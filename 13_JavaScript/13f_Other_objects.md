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


