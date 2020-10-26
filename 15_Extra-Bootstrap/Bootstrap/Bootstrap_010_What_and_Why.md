# Bootstrap 010 -- What is Bootstrap, and Why Use It?

This material is based on Bootstrap version 4.

## What is Bootstrap?

Bootstrap is a framework for CSS.

* *"Responsive"* "Responsive" means it works and adapts across different screen sizes.  It has a "Mobile First" philosophy
* It provides pre-built components people use in CSS such as nav-bars and buttons
* It "fixes" a lot of the annoyances of CSS
* It provides a lot of nice features like grid layout and containers
* Mostly it is a lot of classes

# Versions of Bootstrap

Current version is version 4

# How to include bootstrap

## Download method

* Development
* Minified

### About minimified code

Minified code squeezes out blank spaces, comments, and unnecessary code.  

## Viewport

If you are using Bootstrap, leave in the Viewport meta statement

```html
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
```

## CDN Method

**Content Delivery Network**

A CDN is a server that distributes standardized software

* Conserves Bandwidth: Your website does not have to download specialized software
* Better Load Speed: The software package probably downloads faster because there are usually CDNs located all over the world
* Evem faster load speed:  Your page may not even need to download the software if it is already in cache

CDNs do have downsides

* Danger of code injection, but this is greatly minimized by the "integrity" field
* May load more software than needed
* General insecurity from lack of complete control

## The code you need

```html
<!-- Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">

<!-- Optional theme -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css" integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">

<!-- Latest compiled and minified JavaScript -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
```

## More concise version

```html
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css" integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
```