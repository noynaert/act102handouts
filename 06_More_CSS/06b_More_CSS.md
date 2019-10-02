# 06b More CSS

Here is a limited CSS cheatsheet. http://www.lesliefranke.com/files/reference/csscheatsheet.html

The inside cover of the textbook also has a list of CSS properties. It references pages in the textbook that explain the property.

---

## Properties

---

### *float* and *clear*

Reference: https://www.w3schools.com/css/css_float.asp.  To be honest, float is a property that causes developers to pull their hair out at first.  I suggest starting simple and later use the above link to add sophistication when you need it.

The float property is used to allow text to flow around pictures or blocks of text.  The most common values are *left* and *right.*

IMPORTANT:  You need to use a width of less than the page width to get float to work.  The idea is the floating element has a width of less than the page, and text flows around it!

Here is the amended style.css for highlighting.

```css
.highlight {background-color: bisque;
            float:right;
            width: 30%;
        }
```

Clear undoes the effects of float.  For the exam, just know that clear is almost the opposite of float.

---

## The extremely important "BOX MODEL"

Stuff that may be on the exam: https://www.w3schools.com/css/css_boxmodel.asp

---

### padding

Reference: https://www.w3schools.com/css/css_padding.asp 

* Padding is the space between the edge of the text and the edge of the container.
* The default is 0 padding, so the text on the left and right will slam right against the edge of the container.
* Usually you specify the value for padding as px or em.
* The padding area shares the background color of the element.

```css
.highlight {background-color: bisque;
            float:right;
            width: 30%;
            padding: 0.5em;
        }
```

If you do padding as in the above example, the same amount of padding with be applied to the sides as well as the top and bottom of the element.  You may specify the amount of padding you actually want. on the left, right, top and bottom.  There is also a shorthand available that I do not expect you to learn for the exam.

```css
.highlight {background-color: bisque;
            float:right;
            width: 30%;
            padding-left: 1em;
            padding-right: 0.5em;
            padding-top: 2px;
            padding-bottom:1px:
        }
```

---

### border

Reference: https://www.w3schools.com/css/css_border.asp

Borders can be complex, so start simple and add sophistication as you need it.

A border is immediately outside padding, if any

* border-width is specified in the usual measures.  1px is common.
* border-style is one of several values, but the most common is "solid"
* border-color is any standard color.  If not specified, the color of the element is used.

```css
.highlight {background-color: bisque;
            float:right;
            width: 30%;
            padding-left: 1em;
            padding-right: 0.5em;
            padding-top: 2px;
            padding-bottom:1px:
            border-width: 1px;
        }
```
#### Shorthand border property

```css
            border: 1px solid black;
```
---

### margin

Reference: https://www.w3schools.com/css/css_margin.asp

* Margins are *outside* the border
* Margins take the color of the container, not the element
* Adjacent margins overlap.  For example, if an element has a bottom margin of 15px and the item below it has a margin of 10px, then you might expect a total margin of 25px.  But the margins overlap, so the margin would actually be 15px.  


#### Using Margin properties to center an element

There really is "One wierd trick" to centering text.  Basically the 0 means set the top and bottom margins to 0 (no margin, at the top or bottom, and automatically balance the left and right margins.) The width may be anything less than 100%.

```css
  margin: 0 auto;
  width: 50%;
```

---

## Pseudo properties

---

Technically the :hover plinks.roperty may be applied to any element.  However, it usually is used for 

### :hover

Hover applies when the mouse hovers over an element but no button is pressed on the mouse.

### :active

Active applies when the left mouse button is pressed, but before it is released.

```css
a:hover{color:red;}
a:active{color:blue;}

li:hover{color:red;}
li:active{color:blue;}

*:active {color:green;}
```

---

## Cutting loose

By this point you should be familiar with the basics of CSS.  You may use tags that we have not used in class if they are on the cheatsheet or on the last page of the textbook.  We have not yet covered things like fonts, but we will get to that.  You may have to research how to use some tags on your own.
