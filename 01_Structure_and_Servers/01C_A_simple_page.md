# 01C A Simple Page

## HTML file Structure

```html
<!DOCTYPE html>
<html lang="en-us">
  <head>
    <meta charset="UTF-8">
    <title>Basic Skeleton for html5</title>
  </head>
<body>

</body>
</html>
```
## Fixing the ```<title>```

Give the title something meaningful.

## Puting content in the ```<body>```

At this point the web page is a big white box.

There are many things we can put in it, but for now we are going to focus on headings and paragraphs.

### Headings

We indicate headings with pairs of tags.  The most important tag is ```<h1>...</h1>```. It is pretty common to only have 1 ```<h1>``` tag on a page.  A lot of times the text inside the ```<h1>``` tag matches the title, but it does not have to.

The ```<h2>...</h2>``` tag is the second most important heading.  It would be common to have a lot of ```<h2>``` tags.

### Paragraphs

The pair of tags ```<p>...</p>``` is used to mark paragraphs.

## Word Wrap

The browser handles word wrap.  It is based on the width of the display.  Don't try to control it with the carriage return.

## White Space

The term "White Space" refers to characters like spaces, tabs, and carriage return.  

The browser "collapses white space."  If there are white spaces next to each other, they are collapsed into a single space.

The browser collapses white space before it does word wrap.