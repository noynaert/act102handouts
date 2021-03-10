# 07.80 Favicon

Favicons are the little image that shows up to the left of the URL in the browser. 

Originally they were always named favicon.ico.  But now .pngs and other types.

Modern browsers can generally use any size.  However, 32x32 is generally the optimal size on modern systems. 16x16 is also used sometimes.

One easy way to generate them is a Unicode emoji plus an icon generator such as https://favicon.io/favicon-generator/

The easiest way to get a favicon is to put a file named favicon.ico in the root folder of the server.

The other way is to include one of the following in the &lt;head> of the document.

```html
<link rel="icon" type="image/png" href="http://example.com/myicon.png">
```

You may skip the type="image/png" if you use an .ico file.  The following would pull the favicon from your images folder.

```html
<link rel="icon" href="images/favicon.ico">
```
