# Unit 07_35 Horizontal Menu

```css
    #nav {
      width: 100%;
      float: left;
      margin: 0 0 1em 0;
      padding: 0;
      background-color: #f2f2f2;
      border-bottom: 1px solid #ccc;
    }

    #nav ul {
      list-style: none;
      width: 80%;
      margin: 0 auto;
      padding: 0;
    }

    #nav li {
      float: left;
    }

    #nav li a {
      display: block;
      padding: 8px 15px;
      border-right: 1px solid #ccc;
      text-decoration: none;
      color: #006699;
      text-align: center;
    }

    #nav li a:hover {
      color: #cc0000;
      background-color:#ffffff;
    }

    #nav li:first-child a {
      border-left: 1px solid #cccccc;
    }
```

```html
    <div id="nav">
    <ul id="navigation">
      <li><a href="#campus">Campus</a> </li>
      <li><a href="#mascot">Max Griffon</a></li>
      <li><a href="#logo">The Logo</a></li>
    </ul>
  </div>
```
