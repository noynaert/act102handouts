# 06a More tags and attributes

## The *class* attribute

The *class* attribute is similar to the *id* attribute.  The difference is that many elements on the page may have the same value for the class name.  This allows the same CSS rule to be applied to several different elements on the page.

```html
<p class="important">Do not save your password in plain text.</p>
<p>You should visit <a href="security.html" class="important">this security website</a> before you go on vacation.</p>
<ul>
   <li class="important">Pizza<li>
   <li>vegetables</li>
</ul>
```

### Classes in CSS

In CSS class names have a period in front of them.

```text
.important {color:#FF0000;}
```

### Class names

The rules for class names is similar to the rules for ids.

* Class names should be short and meaningful.  
* Class names may not contain blanks.  
* All lower case letters is recommended.

This is a subtle point, but class ids should describe the content, not the style you plan to use.  For example, suppose that you had decided that all important items on your page would be red.  In this case something like "important" would be a better class name than "red."  The reason is that if you ever decide to change the way important material is highlighted, then you will be stuck with the name "red" even though red may no longer describe the style rule.  This is the type of thing that will make future developers hate you when they have to maintain your page.  It is even worse when that future developer is you.

### Multiple classes

It is possible for an element to have be in more than one class.  In that case, the second (and third) class are separated by blank spaces.  Note that it is blank spaces, not commas.  Does it make sense that classes cannot have blank spaces?

```html
<ul>
   <li class="important food">Pizza<li>
   <li class="food">vegetables</li>
   <li class="important">first aid kit</li>
</ul>
```

### In CSS

In a stylesheet, classes are indicated by putting a period in front of the class name.

## Images

The next unit will focus on images, but they will be introduced here as part of CSS.

### The &lt;img&gt; Tag

The &lt;img&gt; tag is a self-closing tag.

The &lt;img&gt; tag should always have two attributes:

* src="filename" -- This is the name of the file.  Often images are put in a folder called "images."  If the folder is used, the folder must be included in the file name.
* alt="description" -- This is a brief description of the image.  In modern browsers it is often used by screen reading software used by people with impaired vision.

It is also common to include an #id or a .class attribute.

There are other attributes that may be included, such as width.  However, many of these attributes are properly done in CSS rather than the &lt;img&gt; tag itself.

#### Examples of the &lt;img&gt; tag

The first example shows how to do an image in the same folder.  The second shows the preferred method of putting the images in a folder called "images.  There is no magic or "syntax in the directory name of "images."  It is just a standard name used by many developers out of convention.

* &lt;img src="kitten.jpg" alt="Picture of a cute kitten">
* &lt;img src="images/kitten.jpg" alt="Picture of a cute kitten">

## The &lt;div&gt; Tag

The &lt;div&gt;&lt;/div&gt; tag is a paired tag.

Reference: https://www.w3docs.com/learn-html/html-div-tag.html

The &lt;div&gt; tag is kind of like a &lt;section> tag.  In fact, the &lt;section> tag is an addition in html5 that was not available in previous versions.  Before html5 we just used &lt;div&gt; tags and gave them an id.  That is how we marked sections.  

Unlike the &lt;section> tag, there is no rule that an <h?> tag follow.  Also, one &lt;div&gt; tag may appear inside another &lt;div&gt; tag.

The &lt;div&gt; tag is a "container" tag.  It can group together a bunch of paragraphs, headings, images, and lists.

There is always a blank line placed before and after a &lt;div> tag.

```html
<section id="food">
<h2>Foods of Kansas City</h2>
  <div id="bbq" class="sidebar">
    <h3> Kansas City Barbeque Ribs</h3>
    <p>Kansas city is famous for its barbequed foods.</p>
    <img src="ribs" alt="Picture of barbequed ribs">
  </div>
  
  <p>Kansas City has many foods it is known for.</p>
  <!-- Section continues -->
</section>
```

## The &lt;span&gt; Tag

The  &lt;span&gt;  &lt;/span&gt; is a paired tag.

Reference: https://www.w3schools.com/tags/tag_span.asp

The span tag is only used withing paragraphs or lines.  It marks out a very small bit of text that needs special style or other type of attention.

```html
<p><span class="hero">Bill</span> considers <span class="food">Pizza</span> an essential camping supply. <span class="hero">Bill</span> is not very good at camping.</p>
```
