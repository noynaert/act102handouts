# 06_30 Float and Clear

## ```float```

Reference: https://www.w3schools.com/css/css_float.asp.  To be honest, float is a property that causes developers to pull their hair out at first.  I suggest starting simple and later use the above link to add sophistication when you need it.  Or learn to use {display:flex;}

The float property is used to allow text to flow around pictures or blocks of text.  The most common values are *left* and *right.*

IMPORTANT:  

* You need to use a width of less than the page width to get float to work.  The idea is the floating element has a width of less than the page, and text flows around it!  
* Float only works with block elements.  This can be a problem floating images unless they are declared blocks.

## ```clear```


Clear undoes the effects of float.  It is possible to do ```clear:left``` or ```clear:right``` but in most cases we do ```clear:both```.
