# Structure of a web page

This unit corresponds roughly to the following references:

* Duckett textbook: Chapter 1
* W3 Schools
  * https://www.w3schools.com/html/default.asp
  * https://www.w3schools.com/html/html_intro.asp
  * https://www.w3schools.com/html/html_editors.asp (I disagree with them.  I recommend VS Code)
  * https://www.w3schools.com/html/html_basic.asp
  * https://www.w3schools.com/html/html_elements.asp (I called them tags.  W3C calls them elements.)
  * https://www.w3schools.com/html/html_attributes.asp (You don't need to know the attributes they list right now, but you will need to know them eventually.  We will cover the attributes they list later.  For now just know what an attribute is and its basic syntax of an attribute.)

## Of Files and Folders

### Files

We will be working with text files with an extension of .html

#### Two Great Commandments in this course

First Commandment: *Thou shalt not put blanks in file names.*

And the Second Commandment is like unto the first: *Thou shalt not put special characters in file names, except maybe an underscore*

|Good Names|Bad Names|
|---|---|
|index.html|start page.html|
|quick_and_easy.html|quick&easy.html|

### Folders

* Folders, Directories, Subdirectories all mean the same thing.
  * A folder is a collection of files and other folders
  * Windows, Linux, and Mac all use folders to keep things organized
* We will work with folders a lot this semester.  Visual Studio Code works best when it is working with files inside folders.

#### The "Landing Page"

When we view a folder in a browser we can see all of the files.  For example, go to [https://webservices.missouriwestern.edu/users/noynaert/act102/](https://webservices.missouriwestern.edu/users/noynaert/act102/)   You should be able to see the files and folders.

Now go to [https://webservices.missouriwestern.edu/users/noynaert/act102/zzzIgnoreThis/](https://webservices.missouriwestern.edu/users/noynaert/act102/zzzIgnoreThis/)

You cannot see the contents of the zzzIgnoreThis folder because it has a special file named index.html.  index.html is a "landing page."  When you go to a directory or folder with an index.html file the browser shows you the contents of the index.html file instead of the directory contents.  Some systems use names like index.php or default.html.  However, all of these alternate names would be landing pages if they are set up to show by default.

### Editors

We need an editor that is good at processing simple text files

Recommended Editor is [Visual Studio Code](https://code.visualstudio.com/).  It is a free program from Microsoft.  It runs on Windows, Linux, and Mac.

#### The third great commandment of this course:  In VS Code, open folders, not files

Notepad++ is an older editor that will also work for this course, but it lacks a lot of features.

Plain old Windows Notepad will work, but I do not recommend it, except in an emergency editing situation.

### Editors you should not use:

* Wordpad
* Word
* Any other editor that does text formatting in a gui environment.

## Browsers

Browsers are ***Client Software***.  A browser's job is to read an .html file (or other type of file) and "render" it according to the html instructions.

Common Browsers:

* Chrome
* Firefox
* Internet Explorer
* Edge
* Safari
* Opera
* Lynx (Ok, not so common, but interesting)

## HTML file Structure

```html
<!DOCTYPE html>
<html lang="en-us">
  <head>
    <meta charset="UTF-8">↩
    <title>Basic Skeleton for html5</title>
  </head>
<body>

</body>
</html>
```

### &lt;!DOCTYPE html&gt;

The &lt;!DOCTYPE html&gt; statement is not really HTML.  It is just a message to the browser that tells what type of file is coming.

### Tags

Tags describe the structure and function of the text in a document.
Tags are surrounded by "angle brackets."  The are actually the less than and greater than symbols, but are referred to as angle brackets in HTML.

Tags are always in lower case.

Most (but not all) tags come in pairs.  There is an opening tag and a closing tag.  The closing tag always has / before the tag name.

### Tags must be properly nested

Pairs of tags can be nested inside other tags.  In the example code above notice:

* The &lt;html&gt; tag is the first tag, and the &lt;/html&gt; closing tag is the last tag.  Everything else is nested inside.
* The &lt;head&gt; and the &lt;/head&gt; are inside the html tag.  The &lt;/head&gt; appears before the &lt;body&gt; tag starts
* The &lt;title&gt; tag is nested inside the &lt;head&gt; tag.

### How the HTML file is interpreted by the Browser

The "Head" part of the document has "meta" information about the page, including the title.

The text in the &lt;title&gt; is what goes in the browser tab.

The &lt;body&gt; through the &lt;/body&gt; part of the document shows up in the main window.

## Attributes

Sometimes tags have additional information added to them.  The &lt;html lang="en-us"&gt; tag has some extra information tacked on.  The part that says lang="en-us" is called an ***attribute***.  In this case the attribute tells the browser that this page is written in English, and specifically US English.  The browser can use this information to determine which alphabet to use.  If the language had specified Russian, the browser would use a Cyrillic script.

### Attribute format

Attributes always have the same format.  They start with a key work like "lang".  Then they have an equal sign.  Last they have the value.  Normally the value is enclosed in quotation marks.  HTML5 technically does not require quotes if the attribute is a single word, but the convention is to always use the quotes.

There is one other tag that has an attribute.  What is it?

#### Special Note On Oddball Computer Science Jargon

In Computer Science jargon, the " symbol is often called "Double quotes" or "Double quote marks."  We use this terminology because the apostrophe symbol ' is sometime used as quote marks as well.  What normal humans sometimes call an apostrophe is known as a "Single quote" by Computer Scientists.  In most language there are subtle but important differences between a single quote and a double quote.
