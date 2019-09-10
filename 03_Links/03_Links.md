# Links

I recommend the textbook on this unit.  It covers all of the important cases.

There is only one tag in this unit, the &lt;a&gt; tag.  It has one attribute, href.  However, there are several subtle aspects of using the tag.

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
