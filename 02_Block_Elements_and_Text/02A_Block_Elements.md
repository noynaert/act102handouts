# Block Elements

## References

The material in this unit covers roughly chapter 2 of the Duckett textbook.

* Block Elements: [https://www.w3schools.com/html/html_blocks.asp](https://www.w3schools.com/html/html_blocks.asp)
* Headings: [https://www.w3schools.com/html/html_headings.asp](https://www.w3schools.com/html/html_headings.asp)
* Paragraphs: [https://www.w3schools.com/html/html_paragraphs.asp](https://www.w3schools.com/html/html_paragraphs.asp)
* Horizontal Rule (a horizontal line): [https://www.w3schools.com/tags/tag_hr.asp](https://www.w3schools.com/tags/tag_hr.asp)
* Break: [https://www.w3schools.com/tags/tag_hr.asp](https://www.w3schools.com/tags/tag_hr.asp)
* Preformatted: [https://wwwhttps://www.w3schools.com/tags/tag_pre.asp.w3schools.com/tags/tag_pre.asp](https://wwwhttps://www.w3schools.com/tags/tag_pre.asp.w3schools.com/tags/tag_pre.asp)
* Section: [https://www.w3schools.com/tags/tag_section.asp](https://www.w3schools.com/tags/tag_section.asp)
* Id: [https://www.w3schools.com/tags/att_id.asp](https://www.w3schools.com/tags/att_id.asp)
* Footer: [https://www.w3schools.com/tags/tag_footer.asp](https://www.w3schools.com/tags/tag_footer.asp)
* Validation: [https://html5.validator.nu/](https://html5.validator.nu/)

So far we have talked about "tags."  Tags are surrounded by &lt; and &gt; symbols.  Tags are one type of "element."  The name inside the &lt; and &gt; symbols is the element.  For example, ```<body>``` is a tag, but ```body``` is the element.

There are other types of elements, but for right now we can treat elements and tags as the same thing.

Block elements (and block tags) have a blank line before them and after them.

## Headings

* Headings run from ```<h1>``` through ```<h6>```
* ```<h1>```
  * ```<h1>``` is the largest heading
  * ```<h1>``` text is often the same as the text in the ```<title>```
  * ```<h1>``` is the first item on many web pages
  * Some style guides only recommend one ```<h1>``` per page.
* ```<h2>``` through ```<h6>``` should be used like an outline.  Don't jump around randomly.

Remember that html describes the structure of the document.  Don't pick heading levels based on how they look.  If you want a different size or look, then use style sheets (to be covered soonish).

## Paragraphs

* The ```<p>``` tag is a block tag that is used to define paragraphs.  Like other block tags the paragraph tag puts a blank line before and after the paragraph.
* The browser handles word wrap.  Do not try to control it.
* The browser also tries to "collapse white space."
* Do not try to indent the first line of the paragraph.

## Horizontal Rule

The ```<hr>``` tag is a self-closing block tag.  It just draws a solid line across the page or its container.

---

## Break

Technically the ```<br>``` tag is not a block element.  It simply causes a "Break" or carriage return at the point where the ```<br>``` tag occurs.

Break is sometimes used when displaying data.  But use it sparingly.

## Notes about "whitespace"

There are officially 5 whitespace characters:

* ***SPACE*** (the space bar)
* ***TAB*** (the Tab key)
* ***CARRIAGE RETURN*** (or CR, the Enter key)
* ***FORM FEED*** (or FF.  This is typically not important in web pages)
* ***LINE FEED*** (or LF. This is typically not important in HTML or in Windows systems.)

Whitespace is a concept that pops up in a lot of technical forums.  In the context of HTML and programming it refers to characters that do not put ink on the page.  

Form Feed is important in some applications. It generally refers to sending a signal to kick out a new sheet of paper on the printer. FF typically is not important on web pages because web pages are not usually broken up into individual sheets of paper.

Carriage Return and Linefeed are sort of a pair.  The concepts go back to the old days of typewriters and teletype machines.  The CR sends the "carriage" back to the left on a typewriter or teletype.  On a screen it generally means moving the cursor to the left margin.  LF on a paper system means moving down to the next line.  Windows computer systems typically combine both the CR and LF into just the CR.  However, on Macs and Linux systems they tend to be treated as two different operations.  This can cause problems when moving text file (like .html files) between systems.  

### Whitespace in HTML

In html, whitespace characters are "collapsed."  If an html file has more than one whitespace character together the browser will change them into a single space.  The browser then handles word wrap automatically.

## Preformatted

The ```<pre>``` tag is a block element tag.  It does two things:

1. It changes to a fixed or monospaced font
2. It preserves whitespace.

The ```<pre>``` tag has a lot of uses:

* Displaying data in the form of tables
* Displaying things like poems
* Displaying "ASCII Art" if you are a real geek.

```text
     /\_/\
    ( o.o )
     > ^ <
```

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

We will use the validator at [https://validator.w3.org/nu/](https://validator.w3.org/nu/)

There are three ways to validate your web page

1. By URL -- This is the easiest.  The url you copy paste must start with http:// or https://
2. By file upload.  Use this if you have not got the current copy of your document on the Internet yet.  The url probably starts with File:///
3. By text.  This also works in the situation where you are working from your PC.  "Ctrl-A" as a keyboard shortcut is your friend if you are using this.
