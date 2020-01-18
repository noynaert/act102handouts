# Block Elements

## References

* Block Elements: [https://www.w3schools.com/html/html_blocks.asp](https://www.w3schools.com/html/html_blocks.asp)
* Headings: [https://www.w3schools.com/html/html_headings.asp](https://www.w3schools.com/html/html_headings.asp)
* Paragraphs: [https://www.w3schools.com/html/html_paragraphs.asp](https://www.w3schools.com/html/html_paragraphs.asp)
* Horizontal Rule (a horizontal line): [https://www.w3schools.com/tags/tag_hr.asp](https://www.w3schools.com/tags/tag_hr.asp)
* Break: [https://www.w3schools.com/tags/tag_hr.asp](https://www.w3schools.com/tags/tag_hr.asp)
* Preformatted: [https://wwwhttps://www.w3schools.com/tags/tag_pre.asp.w3schools.com/tags/tag_pre.asp](https://wwwhttps://www.w3schools.com/tags/tag_pre.asp.w3schools.com/tags/tag_pre.asp)
* Section:
* Id:
* Footer:
* Validation: [https://html5.validator.nu/](https://html5.validator.nu/)

"Elements" means about the same things as "tags."  Technically, tags have &lt; and &gt; symbols around them.  Elements are just the name.  For example, ```<body>``` is a tag, but ```body``` is the element.

Block elements (and block tags) have a blank line before them and after them.

## Headings

## Paragraphs

## Horizontal Rule

## Break

Technically the ```<br>``` tag is not a block element.  It simply causes a "Break" or carriage return at the point where the ```<br>``` tag occurs.

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
