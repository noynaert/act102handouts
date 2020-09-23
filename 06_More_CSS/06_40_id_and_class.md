#06_40 ```id``` and ```class``` attributes

## The ```id``` attribute

We have already been using id's.  But let's review

* An id may be used only once on a page
* **The value of an id may not have a blank space***
  * A blank space separates ids.  The following creates 3 ids called "food" "and" "drinks"
```     <div id="food and drinks">```
* Recommendations:  
  * Use lower case
  * Keep them short but descriptive of the content

## The ```class``` attribute

The *class* attribute is similar to the *id* attribute.  The difference is that many elements on the page may have the same value for the class name.  This allows the same CSS rule to be applied to several different elements on the page.

```html
<p class="important">Do not save your password in plain text.</p>
<p>You should visit <a href="security.html" class="important">this security website</a> before you go on vacation.</p>
<ul>
   <li class="important">Pizza</li>
   <li>vegetables</li>
   <li class="important">first aid kit</li>
</ul>
```

### Classes in CSS

#### "dot" and "period" 

We have previously seen that computer science people often have different names for punctuation.  For example, they tend to call an apostrophe a "single quote."

Here is another example:   A "period" is often called a "dot."  In normal usage a period almost always comes at the end of something.  However, computer people tend to put their dots everywhere except at the end.

In CSS class names have a period in front of them.

```text
.important {color:#FF0000;}
```

### Class names

The rules and recommendations for class names is similar to the rules for ids.

* A class may be used more than once on a page
* **The value of a class may not have a blank space***
  * A blank space separates class names.  The following creates 3 classes called "food" "and" "drinks"
```     <div class="food and drinks">```
* Recommendations:  
  * Use lower case
  * Keep them short but descriptive of the content
  * Describe the role of the content, not how it looks.

This last item is a subtle point, but class names should describe the content, not the style you plan to use.  For example, suppose that you had decided that all important items on your page would be red.  In this case something like "important" would be a better class name than "red."  The reason is that if you ever decide to change the way important material is highlighted, then you will be stuck with the name "red" even though red may no longer describe the style rule.  This is the type of thing that will make future developers hate you when they have to maintain your page.  It is even worse when that future developer is you.

### Multiple classes

It is possible for an element to have be in more than one class.  In that case, the second (and third) class are separated by blank spaces.  Note that it is blank spaces, not commas.  Does it make sense that classes cannot have blank spaces?

```html
<ul>
   <li class="important food">Pizza<li>
   <li class="food">vegetables</li>
   <li class="important">first aid kit</li>
</ul>
```

## In practice

In practical usage, id's are important because they are unique.  They tend to be most used in defining page structure and function.  Programs that interact with your page tend to use id's more than classes.

In practical usage, classes allow the designer to unify a website with similar graphic design.  Classes tend to be more important in CSS.