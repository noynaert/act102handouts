# CSS and Colors Introduction

Quickstart for this unit:

Add the following line to the head of your document:

```css
 <link rel="stylesheet" href="style.css">
```

Now, in the same folder as your html, create a file named "style.css"

## CSS

CSS stands for "Cascading Style Sheet"  CSS is used to control the appearance of a document.

The syntax of CSS is entirely different than html.

CSS consists of a series of rules that govern how different parts of a document are arranged.

## Syntax of a rule

![Syntax of a CSS rule](images/css.png)

## Selectors

 Selector: The selector specifies what parts of a page the rule will apply to.  A selector can be a lot of different things, but for this unit we will limit the selector to the following:

* an html element such as body, h1, p, a, or hr.  Any element will work.  Remember that an element is the text within the tag
* an id.  You must put # in front of the id.  For example #geography
* A list of selectors with *commas* in between.  An example would be ```h1, h2, h3```.  The style applies to all of the elements listed.
* Two or more selectors with a *space* in between. The style applies to the second element, but only when it is within the first elefment.  For example, ```#cities p``` would only apply to &lt;p&gt; tags within #cities.
  
### Other Selectors
  
There are a lot of selectors.  See [https://www.w3schools.com/ cssref/css_selectors.asp](https://www.w3schools.com/cssref/css_selectors.asp) for the full list

You will not need to know them all.  For now be aware of the list.  

Learning how to read the list is important.

## Properties
* color:  The color to be given to the text
* background-color: uh, the background color
* width: The width of the item.  There are a lot of ways to measure width.  Here are a few
* border: The way a line around the element looks
  
### Values of properties

Different properties take different properties.  

Most properties take a single property, but some take more than one property.  There are a few properties that do not take a value at all.

Sometimes there are different ways to specify a value for a property.  For example, colors may be specified by name, such as "red" but we frequently use numbers such as #123456.

Punctuation in the values can be picky.  Even spaces can be important.

#### Specifying size

Width and height related properties can be specified in several ways.  Here are some of the major methods:

* Pixels: px
  * A pixel is a dot on the screen.  Roughly.
  * Specifying in px can tie the sizes you specify to the screen the user is using.
  * 1px is generally used as the smallest visible size
* Percentage: %
  * Tied to the size of an element's *container*
    * May be the width of the screen
    * If an element is inside another element, it is the size of parent's container
* Em: em
  * An "em" is the size of a square box drawn around a capital letter "M"
    * It is a square box that includes things like spacing and room for descenders
    * em varies on the page by font and also the size of the font
    * It is good when you want something to scale with the page size
    * In practical terms, it is pretty big
    * Examples:
      * 1em
      * 2em
      * .5em <!-- Half an em -->
      * 1.5em <!-- One and a half ems -->

### Other Properties

* Property: There are a lot of properties. In this unit we will only cover a few. See  [https://www.w3schools.com/cssref/](https://www.w3schools.com/cssref/) for a full list.

#### Rule punctuation

Curly braces { } surround the properties in a rule.

A colon : goes between the property and the values

The semicolon ; separates rules. If there is only one rule you do not need to put the semicolon at the end, but it is a good idea to do so.

### Examples of Rules

```css
p {color: blue;} <!-- Turns all text on a page blue -->

h1, h2 {background-color: yellow;
        color: green;
        width: 50%
       }     <!-- I didn't say it was pretty -->

#geography { width: 50% }

hr { color: #123abc}

section {border: 1px solid black;}

```

### Order of Rules and Properties  -- The *Cascade*

The order of the Rules and Properties generally does not matter.  At least in this course, the order only matters if there is a conflict between two rules or two properties. 

Conflicts are resolved by the cascade.  For now the only cascade guideline that matters is that if there is a conflict, the last specification controls.

## CSS placement

CSS rules may go in several places

* In a separate file.  This is what we will use for now.  The other locations may be slightly easier on small projects, but get in the habit of using a separate file
* In a &lt;style&gt; &lt;/style&gt; tag in the &lt;head&gt; &lt;/head&gt; of a document.  This location is really only suitable for websites with a single page.
* inline inside a tag (no selector is needed).  The style= attribute is used.  This location should be used only in very rare circumstances. 

## Linking the HTML file and the CSS file

If the stylesheet is called "style.css" and is in the same directory (folder) as the html file, then the following line should be placed in the &lt;head&gt; of the html document

```html
<head>
  <meta char-set="utf-8">
  <link rel="stylesheet" href="style.css">
  <title>Demo of Styles</title>
</head>
``` 
The order of the statements in the head does not matter.

## Comments

* The one bit of common syntax shared by html and css is comments.  Comments are specified by <!-- Comment goes here --->
* Comments do not show up to the user
* Excessive (or any) comments are discouraged because of bandwidth
* Don't just comment out "dead" or non-working parts of your program and leave them.

