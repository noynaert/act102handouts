# 03F HTML Entities

References:

* https://www.w3schools.com/html/html_entities.asp
* Reference for entities: https://dev.w3.org/html5/html-author/charref
* Another entity reference: https://www.freeformatter.com/html-entities.html
* Unicode Emogis https://unicode.org/emoji/charts/full-emoji-list.html
* Emogi reference: https://emojipedia.org/

## Some special cases

### The problem of ```<```

Suppose you need to create the following line on a web page:

```5 < 10```

The &lt; symbol is going to be a problem.  The browser will see the less than symbol as the start of a tag.

The solution is an "HTML Entity"  Instead of the less than symbol, use &amp;lt;  

### The problem of the &

Now we have another potential problem.  What happens if we need an ampersand?   The solution is an entity for the ampersand.  It us &amp;amp;

### Other common problems

Suppose we need a character that is not on the keyboard?  Something like &copy; for copyright, &cent; for cent, or  &infin; for infinity.

### The most commonly used entity -- The "Non-breaking Space"

The &nbsp; is possibly the most important of the entities.

Visually, the non-breaking space looks just like a space.  That is, it is invisible.  It has an Extended ASCII code of 255.

Technically, the nbsp keeps words "stuck together" so they will not word wrap when they occur at the end of a line.  For example, if you don't want "Missouri Western" to split across lines.  

But in html, it serves some other purposes.

* To avoid collapsing white space. The browser collapses white space.  However, the nbsp is not considered white space, so it does not collapse.
* As a placeholder or "peg."  Some HTML tags need some "printable" content.  One example is a blank cell in a table (at least on older browsers).  Simple blank spaces will not work.  But the nbsp does work.
* As a placeholder that will be replaced by JavaScript.  Later in the course we will look at JavaScript.  One thing we commonly do with JavaScript is to fill in data at the time the page is in use.  

## Three forms

HTML entities always start with an ampersand (&) and ends with a semicolon (;).

## Pneumonic

The most common entities have a pneumonic form.  So far we have used a short sequence of letters that are fairly easy to remember.  "lt" for "less than," "amp" for "ampersand", "copy" for "copyright,"  "cent for "cent," and "inf" for "infinity."

## Entities to know

Symbol|Code|Name
:---:|:---:|:---
&lt;|&amp;lt;|less than
&nbsp;|&amp;nbsp;|nbsp
&copy;|&amp;copy;|copyright
&cent;|&amp;cent;|cent
&euro;|&amp;euro;|Euro
&yen;|&amp;yen;|Yen


## Decimal

HTML Entities may also be specified by decimal values.  In the case of ASCII codes.  The key is to use the "number sign" or "hashtag" symbol,	&#35;.  

An A may be specified as &amp;#65;.

### Hexadecimal

Entities may be specified in hexadecimal.  The key here is to use #x before the hex digits.  

An A may be specified as &amp#x41;

Why use hex?  Often the reference will only list the hex value.  It is usually shorter with the number gets very large.  Also, the hex code does give some information about the structure of the code itself.

#### Decoding the U+ notation

Take a look at (https://unicode.org/emoji/charts/full-emoji-list.html)[https://unicode.org/emoji/charts/full-emoji-list.html].  They specify the characters as things like U+1F600	The part after the U+ is the hex value.  So the &#x1F600; becomes &amp;#x1F600;

## Composites

Composites are combinations of entities, or the combination of a regular character and an entity.

One use of composites is to write diacritical marks on characters.

* a&amp;#768; gives a&#768;
* O&amp;#768; gives O&#768;
* e&amp;#769; gives e&#769;
* O&amp;#769; gives O&#769;
* a&amp;#771; gives a&#771;
* O&amp;#771; gives O&#771;

### Unicode Composites

Unicode composites are somewhat browser dependent.  Unicode flags are generally supported, but be aware that some composites may not be available in all browsers.  Also, different platforms may represent the emojis differently.

Flats are pretty well supported, so we will use them first.  See https://emojipedia.org/flags/  Note that the composit is based on the two-letter country abbreviations.

#### Example of a less-supported emoji :man_cook: :woman_cook:

Note that the Sign for "woman cook" is the symbol for woman (U+1F69) combined with a narrow space (U+200D) and an eggry frying in a pan (U+1FF373)

* :woman: U+1F469
‍* A "Narrow Space" U+200D
* :cooking: U+1F373