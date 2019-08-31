# Text in HTML

# Of Bits and Bytes

* A bit stores a one or a zero

|Number of Bits|Number of Possible Combinatins|Examples|
|:---:|:---:|:---:|
|1|2|0,1|
|2|4|00, 01, 10, 11|
|3|8|000,001,010,011,100,101,110,111|
|4|16|0000,0001,0010,0011,0100,0101,0110,0111,1000,1001,1010,1011,1100,1101,1110,1111}
|5|32|-|
|6|64|-|
|7|128|-|
|8|256|-|

The formula for the number of combinations is 2ⁿ where n is the number of bits.

### Number Systems

* Decimal -- Base 10
* Binary -- Base 2  This is the base used inside the computer
* Hexadecimal or "Hex" -- Base 16

Hex is often used as a shorthand for writing binary.

## Character Sets

* ASCII character set
  * Assigns each character a number
  * [ASCII Table](http://www.asciitable.com/)
  * Basic ASCII codes cover all the alphabetic characters used in English
  * 7 bits, 127 characters.
  * Modern computers use 8-bit bytes.  2⁸ is 256.  So another 127 characters could be added.  A lot of these new characters were for western European characters.

* Unicode characters set
  * ASCII does not serve as an international coding system.
  * [Unicode](http://www.unicode.org/charts/) supports most alphabets of the world as well as special symbols.
  * ASCII lives on as the first code table in Unicode, so ASCII is a subset of Unicode.

## Back at the HTML

Content in this section is also covered in the following references:

* Duckett textbook, chapter 2
* HTML Tutorial content:
  * [Headings, hr](https://www.w3schools.com/html/html_headings.asp)
  * [Paragraphs](https://www.w3schools.com/html/html_paragraphs.asp)
  * [Text Formatting](https://www.w3schools.com/html/html_formatting.asp)
  * [Comments](https://www.w3schools.com/html/html_comments.asp)

## All content must be in a tag

All text must be in a paragraph or some other type of container.

## White Space

White space is any character with an ASCII code of 32 or less.  White space includes blanks, tabs, and carriage returns.  

***HTML collapses all white space to a single white space.  So if you have 10 spaces and a tab, all 11 characters will become a single space.  This is how browsers handle "word wrap."***

## Headers

* &lt;h1&gt; ... &lt;/h1&gt;
* &lt;h2&gt; ... &lt;/h2&gt;
* &lt;h3&gt; ... &lt;/h3&gt;
* &lt;h4&gt; ... &lt;/h4&gt;
* &lt;h5&gt; ... &lt;/h5&gt;
* &lt;h6&gt; ... &lt;/h6&gt;

&lt;h1&gt; is the most important heading.  It often matches the &lt;title&gt;

The headers should be used in order.  Do not pick headers based on appearance (we will use CSS for that).

Nest headers logically.

## Paragraphs

The &lt;p&gt; tags is one of the most common.  It is intended to enclose paragraphs.  

By convention, do not attempt to indent paragraphs.  Note that HTML collapses white space, so at most the paragraph will only be indented by one space.

All browsers will make sure there is a blank line before and after a paragraph

## Character formatting

The following are discussed in the [html tutorial](https://www.w3schools.com/html/html_formatting.asp)  There is also material on them in the Duckett text.

&lt;b&gt; - Bold text
&lt;strong&gt; - Important text
&lt;i&gt; - Italic text
&lt;em&gt; - Emphasized text
&lt;mark&gt; - Marked text
&lt;small&gt; - Small text
&lt;del&gt; - Deleted text
&lt;ins&gt; - Inserted text
&lt;sub&gt; - Subscript text
&lt;sup&gt; - Superscript text

### bold and strong, italics and emphasis

Here we get into a bit of an argument amoung the people who take html very seriously.  Most browsers interpret &lt;strong&gt; as the same thing as **bold.**  Similarly, most browsers interpret &lt;em&gt; as *italics.*  

Remember that html is supposed to represent structure and meaning, not style.  Therefore html purists insist that we should use only &lt;strong&gt; and &lt;em&gt; and never use the &lt;b&gt; and &lt;i&gt;.  On the other hand the &lt;b&gt; and &lt;i&gt; are easier to remember and are clear to human readers.

## Horizontal Rule

The &lt;hr&gt; tag generates a straight line across the page.  It is usually a separator between sections of a document.

### Self-closing tag, and html5

There is no closing &lt;hr&gt; tag.  HR is a "self-closing" tag.

HTML5 allows a tag like &lt;hr&gt;.  Previous versions of html required self-closing tags to be written as &lt;hr /&gt; with a / at the end of the tag.  My fingers may still type self-closing tags like this.  It is allowed in html5, but not required.

## &lt;br&gt; Line Break

The &lt;br&gt; tag is a line break.  It is a self-closing tag.  Normally it goes inside a &lt;p&gt; tag.  The &lt;br&gt; tag is self-closing.

## Non-breaking white space

This is not strictly html.  It is an "html entity."  

ASCII code 255 is a "hard space" or "non-breaking white space."  It looks like a space, but the browser will not try to word wrap on the hard space.   It is represented as **&amp;nbsp;**

Sometimes we use **&amp;nbsp;** to join words we want to split.  But often we use the **&amp;nbsp;** entity to fill a space we want to appear empty.

Also, the **&amp;nbsp;** is not collapsed like regular white space.  So sometimes it is used to space out text into a certain format.

## &lt;pre&gt; Preformatted text

The &lt;pre&gt; tag is for "preformatted text."  The &lt;pre&gt; tag does two things.

1. The font is changed to a fixed width font.
2. Spacing and line breaks are respected.

This can be useful for something like a poem.  It can also be used to present data.

Sometimes people use the &lt;pre&gt; tag to defeat the auto formatting of html.  Do not use the &lt;pre&gt; tag excessively.  There are better formatting options in CSS when we get to that point.

## &lt;!-- Comments --&gt;

Comments do not show up when the browser renders the web page.  They are notes to the programmer, or to people who look at the source code later.

If you take a programming course like Java the instructors want you to put in a lot of comments.  However, in html we do not want a lot of comments.  Comments still have to be downloaded, and that takes bandwidth.  If you have a web page that is being served millions of times a day, then the extra comments can end up costing a lot of money and slowing delivery of your web page.

One other thing.  Do not use comments to block out code that did not work properly.  I will deduct points if you have commented out code in assignments you turn in!
