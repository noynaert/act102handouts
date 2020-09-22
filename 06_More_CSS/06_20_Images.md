# 06 20 Images

The next unit will focus on images, but they will be introduced here as part of CSS.

## Size Matters

Image files can be large.
- Takes bandwidth to download
  - Someone has to pay for it
  - Caps
- Takes longer to download and render
  - Bad user experience
  - Lower Google ranking for your page

### Resizing your images

Image sizes are usually measured in pixels

You may use MS Paint or almost any image editor to resize images.  

Two ways to reduce the size.  (You may do both.)

* Reduce the pixels
* Crop the image

Recommended practice:  put the image size in the file name.

## The &lt;img&gt; Tag

The &lt;img&gt; tag is a self-closing tag.

The &lt;img&gt; tag should always have two attributes:

* src="filename" -- This is the name of the file.  Often images are put in a folder called "images."  If the folder is used, the folder must be included in the file name.
* alt="description" -- This is a brief description of the image.  In modern browsers it is often used by screen reading software used by people with impaired vision.

It is also common to include an #id or a .class attribute.

There are other attributes that may be included, such as width.  However, many of these attributes are properly done in CSS rather than the &lt;img&gt; tag itself.

### Examples of the &lt;img&gt; tag

The preferred method of putting the images is to put all the image files in a folder called "images."  There is no magic or syntax in the directory name of "images."  It is just a standard name used by many developers out of convention.

* &lt;img src="kitten.jpg" alt="Picture of a cute kitten">
* &lt;img src="images/kitten.jpg" alt="Picture of a cute kitten">
