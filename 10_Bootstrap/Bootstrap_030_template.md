# Bootstrap 015 Template
The following is a Bootstratp 5 template.

* Leave in the "viewport" meta tag.  Bootstrap 5 needs it.
* Put the reference to the Bootstrap stylesheet in the head
  * The link to the stylesheet should appear ***before*** any local stylesheets.  This allows the local stylesheets to override Bootstrap defaults
  * I like to put the Bootstrap CDN reference before the &lt;title> tag, and local links and &lt;style> tags after the title.
* The script tag for JavaScript should appear at the end of the body.
  
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
   
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/5.0.0-alpha2/css/bootstrap.min.css" integrity="sha384-DhY6onE6f3zzKbjUPRc2hOzGAdEf4/Dz+WJwBvEYL/lkkIsI3ihufq9hk9K4lVoK" crossorigin="anonymous">

  <title>Bootstrap</title>
  <!-- Local stylesheets go here -->
</head>
<body>


   <script src="https://stackpath.bootstrapcdn.com/bootstrap/5.0.0-alpha2/js/bootstrap.bundle.min.js" integrity="sha384-BOsAfwzjNJHrJ8cZidOg56tcQWfp6y72vEJ8xQ9w6Quywb24iOsW913URv1IS4GD" crossorigin="anonymous"></script>
</body>
</html>
```
