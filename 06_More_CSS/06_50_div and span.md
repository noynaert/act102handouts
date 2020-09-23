# 06a More tags and attributes


---


---

## The &lt;div&gt; Tag

The &lt;div&gt;&lt;/div&gt; tag is a paired tag.

Reference: https://www.w3docs.com/learn-html/html-div-tag.html

The &lt;div&gt; tag is kind of like a &lt;section> tag.  In fact, the &lt;section> tag is an addition in html5 that was not available in previous versions.  Before html5 we just used &lt;div&gt; tags and gave them an id.  That is how we marked sections.  

Unlike the &lt;section> tag, there is no rule that an <h?> tag follow.  Also, one &lt;div&gt; tag may appear inside another &lt;div&gt; tag.

The &lt;div&gt; tag is a "container" tag.  It can group together a bunch of paragraphs, headings, images, and lists.

There is always a blank line placed before and after a &lt;div> tag.

```html
<section id="food">
<h2>Foods of Kansas City</h2>
  <div id="bbq" class="sidebar">
    <h3> Kansas City Barbeque Ribs</h3>
    <p>Kansas city is famous for its barbequed foods.</p>
    <img src="ribs" alt="Picture of barbequed ribs">
  </div>
  
  <p>Kansas City has many foods it is known for.</p>
  <!-- Section continues -->
</section>
```

---

## The &lt;span&gt; Tag

The  &lt;span&gt;  &lt;/span&gt; is a paired tag.

Reference: https://www.w3schools.com/tags/tag_span.asp

The span tag is only used withing paragraphs or lines.  It marks out a very small bit of text that needs special style or other type of attention.

```html
<p><span class="hero">Bill</span> considers <span class="food">Pizza</span> an essential camping supply. <span class="hero">Bill</span> is not very good at camping.</p>
```
```css
.highlight {background-color: bisque;
            float:right;
            width: 30%;
        }
```