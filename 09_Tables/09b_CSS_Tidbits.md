# 09b CSS Tidbits and Inspecting Code

## Videos

* [Part 1 on Selectors](https://mwsu.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=06a71218-31e3-4f2b-8c77-aaeb01675614)
* [Part 2 on Minifying and Developer Mode](https://mwsu.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=71901bab-bbbc-4ec2-b916-aaeb016755ec)

## More Selectors

Review:  Selectors are part of the CSS rule that occurs to the left of the {...} curly braces.  For example, "body" is the selector in the following:

```css
body {width: 85%;}
```

So far we have seen the following selectors:

* element -- An html element such as p, h1, or div
* #id -- The hashtag is used for an id selector
* .class -- The period is used to indicate a class selector
* item1, item2, item3 -- Commas separate a *list* of selectors.  The rule is applied to all elements on a list.  We often use this with tables:

```css
   h2, h3, h4, h5, h6{color:green;}
   table, tr, th, td, caption {border:1px solid black;}
```

But there are many, many other selectors.  The full list is at [https://www.w3schools.com/cssref/css_selectors.asp](https://www.w3schools.com/cssref/css_selectors.asp).  You don't need to know them all.  You may look them up if you need them. But we will add 2 here.

## List without commas

```html
<style>
table caption {border:2px solid blue;}
#cast caption {background-color:mint;}
</style>
...
<table>
  <caption>  <!-- This caption will have a blue border -->
     ...
</table>
...
<table id="cast">
   <caption> <!-- This caption will have a mint background color AND a blue border -->
```

I think it helps to read lists without commas backwards.  The rule only applies to things at the end of the list that are within the thing at the start of the list.  In the above example, the mint background-color will be applied to captions within items with an id="cast" attribute.

## * (asterisk)

The asterisk applies to all elements.

```css
* {background-color: orange;}
table * {border:1px solid black;}
```

By the above css, 

* By the first rule, all elements on the page would have an orange background. 
* By the second rule all items in the table would have a border.  This means *every element*.  So if you had a &lt;ul>&lt;li> in the table they would all have borders.

## Minify

We often add indentation and white space for human readability, but the browser does not need them.  Often the code is "minified" prior to deploying it.

Warning:  If you minify code, make sure you keep an original!

There are many ways to minify code:

* VS Code has multiple extensions that minify.  But I have not found one I like.
* Use websites such as [minifycode.com](http://minifycode.com) uses copy/paste or file upload.  Note that the minifycode site also "beautifies" code which is the opposite of minifying it.
* Many advanced development tools like angular.js have tools that automatically minify code when you deploy it to a live website.

## Developer mode

To go to developer mode in Chrome:

* Method 1
  * Click the three dots in the upper-right corner of Chrome
  * Select "More Tools"
  * Select "Developer Mode"
* Method 2
  * Right click an element on the page (for example an img or h1)
  * Select element

Moving the panel elsewhere

* In the Developer Mode panel itself there are three dots.  Click them.
* There should be a "Dock Side" panel that allows you to move the panel to the side, bottom, or float it.

Firefox has something similar.

### HTML Validator for Chrome (and Firefox)

The HTML Validator is an extension for Chrome that runs within developer mode.

[HTML Validator for Chrome](https://chrome.google.com/webstore/detail/html-validator/mpbelhhnfhfjnaehkcnnaknldmnocglk?hl=en-US)

I found that I had to *completely* close Chrome and then reopen it.  (Right-click on the Chrome icon in the status bar and Quit.)