# 06_60 Pseudo selectors

Technically the :hover property may be applied to any element.  However, it usually is used for anchors and links.

[W3C information](https://www.w3schools.com/css/css_pseudo_classes.asp)

## :hover

Hover applies when the mouse hovers over an element but no button is pressed on the mouse.

## a:active

Active applies when the left mouse button is pressed, but before it is released.

```css
a:hover{color:red;}
a:active{color:blue;}

li:hover{color:red;}
li:active{color:blue;}

*:active {color:green;}
```

## a:visited

:visited applies to links that were previously visited.  Most browsers change blue links to purple after you use them.  :visited is often used to undo this behavior.  It is sometimes a bad thing to do.