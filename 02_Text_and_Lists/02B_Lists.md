# Lists

## References

* [W3 Schools HTML Tutorial](https://www.w3schools.com/html/html_lists.asp)
* Textbook, Chapter 4

## Sections

The &lt;section&gt; tag helps organize the structure of a document by grouping items that are part of the same topic.  It is a paired tag.

### The id= attribute

The id= attribute gives a unique name to a section of the html document.  The name should appear in "double quotes."  The name should be short, simple, and meaningful to a human reader.  ***Each name must be unique within a single html document.***

The section tag should normally have an id= attribute.  The section tag should halso be followed immediately by a header of any level from &lt;h1&gt; through &lt;h6&gt;

And example of a section follows:

```html
 <section id="geography">
    <h2>Geography</h2>
    <p>Saint Joseph is located in Burchanan and Andrew Counties of Missouri.  It is the county seat of Buchanan County.</p>
</section>
```

## Footers

The &lt;footer>&lt;/footer> tag goes at the bottom of your document. Your document may have several footer tags, but they should be the last item in your document right above the &lt;/body> tag.

The footer tag is used for things like listing contact information or sources.

## Validation

***Validate early and often!*** It is easier to validate when you have a little bit of source code.

We will use the validator at https://html5.validator.nu/

There are three ways to validate your web page

1. By URL -- This is the easiest.  The url you copy paste must start with http:// or https://
2. By file upload.  Use this if you have not got the current copy of your document on the Internet yet.  The url probably starts with File:///
3. By text.  This also works in the situation where you are working from your PC.  "Ctrl-A" as a keyboard shortcut is your friend if you are using this.

## Lists

Web pages often have a lot of lists.  So this information is important!

* Lists have two tags that are used together. You may put as much text as you want within a &lt;li&gt; tag.  Word wrap happens automatically, just like paragraphs.
* Lists have to appear outside of paragraphs or headings.  Lists cannot contain paragraphs or headings.
* Any amount of text may appear within the &lt;li&gt; tag.

### Unordered Lists

Here is a list of Missouri Cities as an example.

```html
<ul>
   <li>Kansas City<li>
   <li>Saint Joseph<li>
   <li>Saint Louis<li>
   <li>Springfield<li>
   <li>Tipton<li>
</ul>
```

The HTML tutorial at https://www.w3schools.com/html/html_lists.asp has styling guidelines.  However, I would prefer to do these in CSS rather than incorporate the styling directly to the HTML

### Ordered Lists

Ordered lists are very similar to unordered lists.  Ordered lists are appropriate for situations when there is a natural ordering.

Here is a list of the best movies of all times according to https://www.ranker.com/crowdranked-list/the-best-movies-of-all-time

```html
<ol>
   <li><i>The Godfather</i></li>
   <li><i>Pulp Fiction</i></li>
   <li><i>The Shawshank Redemption</i></li>
</ol>
```

The HTML tutorial explains the use of the type attribute.  Attributes are technically not styling.  Therefore feel free to use them.

Type|Description
:---:|:---
type="1"|The list items will be numbered with numbers (default)
type="A"|The list items will be numbered with uppercase letters
type="a"|The list items will be numbered with lowercase letters
type="I"|The list items will be numbered with uppercase roman numbers
type="i"|The list items will be numbered with lowercase roman numbers

### Definition Lists

Definition Lists are used for special purposes, specifically definitions.  However, they can sometimes be useful for other things.

There are three tags used.

* &lt;dl&gt; are the first and last tags that surround the list.
* &lt;dt&gt; defines the term
* &lt;dd&gt; is for the definition

### Nesting Lists

Sometimes it is necessary to put a list inside a list.

This is the wrong way to do a nested list.  

#### The wrong way to do a nested list

```html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
    <ul>
      <li>Black tea</li>
      <li>Green tea</li>
    </ul>
  <li>Milk</li>
</ul>
```

#### The correct way to do a nested list

The inner list is actually a part of the &lt;li&gt; above it.

```html
<ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea</li>
    </ul>
  </li>
  <li>Milk</li>
</ul>
```