# 02B Text Elements

## References


* Block Elements: [https://www.w3schools.com/html/html_formatting.asp](https://www.w3schools.com/html/html_formatting.asp)

## About Text Formatting

Generally html tags are used to indicate structure and meaning, not how material looks.  But sometimes the way things look is important to the meaning.

When we do CSS we will see that there are more sophisticated ways to change the way characters look, but for now we will focus on the html tags that are involved.

## &lt;b&gt; and &lt;strong&gt;

The &lt;b> tag makes text **bold**.  Most browsers display text in the &lt;strong> tag as bold.

## &lt;i> and &lt;em>

The &lt;i> tag is used to display *italics*.  Most browser display the &lt;em> tag to display italics.

## &lt;mark> 

The &lt;mark> tag usually represents as a <mark>yellow highlighter</mark> run over the text.  But different browsers may treat it differently.

## &lt;del>

The &lt;del> tag usually shows up as <del>strikethrough</del> text.  This is used to indicate that text has been deleted from a document.  It is also a favorite of snarky and passive-aggressive Redditors. 

## &lt;ins>

The &lt;ins> tag indicates text that has been inserted into a draft.  It is usually represented as an <ins>underscore</ins>.

## &lt;sup>

The &lt;sup> tag is used to create superscripts.  It is useful for exponents and similar math notations.  For example, 3<sup>2</sup> would be written as 3&lt;sup>2&lt;/sup>.  The &sup> tag is also useful for producing references to footnotes and endnotes.

## &lt;sub>

The &lt;sub> tag produces subscripts.  

## &lt;large> and &lt;small>

There are tags for large and small.  As you might expect, they increase and decrease the size of the text.  But I discourage their use.  most of the other tags in this section have structural meanings.  However, large and small are simply appearance.  It is better done with CSS.  We will do that later in the course.

## Nesting Tags

The text tags on this page may be nested.  For example it is possible to have both <b><i>bold and italics</i></b>.  The trick is to remember that tags must be properly nested.  The best second tag must be opened and closed inside the first tag.  For example &lt;b>&lt;i>X&lt;/i>&lt;/b>. This is called "First In, Last Out" or LIFO.

The order of the nesting does not matter for these text tags, although the order does matter for some types of nesting.

## Spacing

Be careful of spacing around tags.  You should have blanks if they are needed; the tags do not become blanks.  Also be careful of punctuation around tags.  When you are learning html, be careful to watch the preview.