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

Technically the ```<br>``` tag is not a block element.  It simply causes a "Break" or carriage return at the point where the ```br``` tag occurs.

## A note about "whitespace"

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
