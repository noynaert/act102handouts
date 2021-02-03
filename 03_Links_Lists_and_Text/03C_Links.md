# Links


There are only two new tags in this unit.

## &lt;div>

The ```<div>``` tag is a block element.

The ```<div>``` tag is for "division."  It is similar to the ```<section>``` tag and the ```<footer>```.  Section and footer tags were added in html5.  Before html5 we only used div elements.

The div element may be used to mark part of a document with an id.  The main difference is that the ```<div>``` tag does not need a heading element right after it.  That makes the div element more or less invisible.

Normally the div element will have either an id or a class attribute with it.  Sometimes it has both an id and a class.

```html
<div id=sports>
    <p>You can watch sports on ESPN.</p>
</div>
```

### id rules

This section is really a ghost of semesters past.  IDs are now covered earlier in the course.  The video at this point will not cover IDs, but it would not hurt to review the rules for IDs because there is an exam next week!

* An id must be unique on the page
* Do not put a blank in the id
  * If you create an id such as id="geography and climate" you have actually created three ids named "geography" "and" and "climate"
* Use lower case.  This is not a rule, just a style guide
* IDs should be meaningful, but short and simple

## The basic &lt;a&gt; tag

```html
   <a href="______________________">_____________</a>
```

Think of it as a fill-in-the-blank problem.  The first blank is filled with a location.  Usually it is filled with a url.  The second blank is filled with the text you want the user to see.

```html
<p>You can watch the news at <a href="https://cnn.com">CNN</a>.</p>
<p>Schedule an appointment at <a href="https://noynaert.youcanbook.me">https://noynaert.youcanbook.me</a></p>
```

## Absolute vs relative addresses

URLs are absolute addresses.  You may also give the name of a local file.  The following is an example of a relative reference:

```html
<p><a href="cronkite.html">Walter Cronkite</a> was raised in Saint Joseph.</p>
```

## Going to an id on the same page

Use the #before an ID.

```html
<h2>Table of Contents</h2>
<ul>
  <li><a href="#geography">Geography</a></li>
  <li><a href="#economy">Economy</a>/li>
  <li><a href="#people">Famous Citizens</a></li>
</ul>
```

## Going to an ID on a different page

```html
<h3>About Walter Cronkiite</h3>
<ul>
  <li><a href="cronkite.html#early">Early Life</a></li>
  <li><a href="cronkite.html#WWII">World War II</a></li>
  <li><a href="cronkite.html#space"><The Space Program/a></li>
</ul>
```
