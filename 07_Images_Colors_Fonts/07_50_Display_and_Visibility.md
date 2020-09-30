# 07_20 Display and Visibility

Here is a limited CSS cheatsheet. http://www.lesliefranke.com/files/reference/csscheatsheet.html

The inside cover of the textbook also has a list of CSS properties. It references pages in the textbook that explain the property.

---

## Properties

### display Property

The ```display``` property has many possible values.  The most important ones are shown below.

```css
 {display:block;}
 {display:inline;}
 {display:none;}
 {display:flex;}
```

#### block

A block-level element always starts on a new line and takes up the full width available.  The width of a block defaults to the width of its container.

Examples of tags that are blocks by default:

* &lt;body&gt;
* &lt;p&gt;
* &lt;h*x*&gt;
* &lt;ul&gt;
* &lt;div&gt;
* &lt;section&gt;
* &lt;footer&gt;
* &lt;hr&gt;

#### inline

An inline element does not start a new line.   It only takes up the space required.

It is fairly common to specify some tags like &lt;ul&gt; elements to be inline tags.

Examples of tags that are inline by default:

* &lt;a&gt;
* &lt;span&gt;
* &lt;img&gt;

It is fairly common to specify some tags like &lt;ul&gt; elements to be inline tags.

Some inline tags like the &lt;img&gt; tag are often redefined as block.

#### none

None means that that item is not displayed, *and no room is left for it.*    This contrasts with {visibility:hidden;}  If something is hidden space is reserved for the item, but the space is left appearing empty.

#### flex

Flex is a relatively new value.  We will do a section on it later. [A guide to flex](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

---


#### Using Margin properties to center an element

There really is "One wierd trick" to centering text.  Basically the 0 means set the top and bottom margins to 0 (no margin, at the top or bottom, and automatically balance the left and right margins.) The width may be anything less than 100%.

```css
  margin: 0 auto;
  width: 50%;
```

---



---

## Cutting loose

By this point you should be familiar with the basics of CSS.  You may use tags that we have not used in class if they are on the cheatsheet or on the last page of the textbook.  We have not yet covered things like fonts, but we will get to that.  You may have to research how to use some tags on your own.
