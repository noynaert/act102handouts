# Lists

## References

* [W3 Schools HTML Tutorial](https://www.w3schools.com/html/html_lists.asp)
* Textbook, Chapter 4

Web pages often have a lot of lists.  So this information is important!

* Lists have two tags that are used together. You may put as much text as you want within a &lt;li&gt; tag.  Word wrap happens automatically, just like paragraphs.
* Lists have to appear outside of paragraphs or headings.  Lists cannot contain paragraphs or headings.
* Any amount of text may appear within the &lt;li&gt; tag.

## Unordered Lists

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

## Ordered Lists

Ordered lists are very similar to unordered lists.  Ordered lists are appropriate for situations when there is a natural ordering.

Here is a list of the best movies of all times according to https://www.ranker.com/crowdranked-list/the-best-movies-of-all-time

```html
<ol>
   <li><i>The Godfather</i></li>
   <li><i>Pulp Fiction</i></li>
   <li><i>The Shawshank Redemption</i></li>
</ol>
```

The HTML tutorial explains the use of the type attribute.  However, this style of doing types is obsolete.  Do not use it at this time.  Once we get to CSS we will learn to do the styling in a better way.

## Nesting Lists

Sometimes it is necessary to put a list inside a list.

This is the wrong way to do a nested list.  

### The wrong way to do a nested list

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

### The correct way to do a nested list

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

## Definition Lists

**NOTE:**  *Definition lists will not be on the exam.  You are welcome to use definition lists in assignments, but they will not be on the exam.*

Definition Lists are used for special purposes, specifically definitions.  However, they can sometimes be useful for other things.

Definition Lists are sometimes called "Description Lists."  This reflects the idea that &lt;dl&gt; lists often include more than just definitions.

There are three tags used.

* &lt;dl&gt; are the first and last tags that surround the list.
* &lt;dt&gt; defines the term
* &lt;dd&gt; is for the definition

### Example of a Definition List

From Greek mythology:

```html
<dl>
    <dt>Argus</dt><dd>A hundred-eyed giant.</dd>
    <dt>Centaur</dt><dd>A creature with the head and torso of a human and the body of a horse</dd>
    <dt>Griffon or Gryphon</dt><dd>A creature with the head of a lion and the body and wings of an eagle.  They were guardians of gold, and were generally rather disagreeable creatures.</dd>
  </dl>
```

It would look like this:

<dl>
    <dt>Argus</dt><dd>A hundred-eyed giant.</dd>
    <dt>Centaur</dt><dd>A creature with the head and torso of a human and the body of a horse</dd>
    <dt>Griffon or Gryphon</dt><dd>A creature with the head of a lion and the body and wings of an eagle.  They were guardians of gold, and were generally rather disagreeable creatures.</dd>
  </dl>