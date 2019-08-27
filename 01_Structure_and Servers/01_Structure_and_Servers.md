# Structure of a web page

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

### Editors

We need an editor that is good at processing simple text files

Recommended Editor is [Visual Studio Code](https://code.visualstudio.com/).  It is a free program from Microsoft.  It runs on Windows, Linux, and Mac.

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
<html>
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

