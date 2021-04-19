# 11.050 Objects

Objects are another composite data type like arrays.  Arrays are basically lists of items.  In objects, each of the individual values has a name, and the order doesn't matter.

Indicate the entire object with the name of the object.  

Indicate the individual fields by using the object name followed by a period, then the field name.

* Objects may contain values
* Objects can contain functions
* Object may contain arrays or other objects

Each part of the DOM is an object.  We usually manipulate the DOM by manipulating the various objects.

```javascript
function changePicture(fileName){
  let picture = document.getElementById("fred");
  picture.src=fileName;
}
...
<img id="fred" src="images/start.jpg" alt="">
<button onclick="changePicture('images/second.jpg')">
```

##  `document.getElementById("id")`

The "document" in `document.getElementById()`  refers to the DOM.

The function getElementById() is one method in the document object.

getElementById() is used more than getElementByClass() because getElementById only gets one item.  When you getElementByClass you get back an array, even if there is only one instance of the class on a page.  (Why?  That would make a good question on the final exam, I think.)

## JSON

JSON is a string representation of JavaScript Objects.  It is widely used to exchange data  between programs.  It is a string, and almost all computer languages can process strings.  Most current languages have the ability to read and write JSON files.

