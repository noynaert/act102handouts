# 11.040 This and That

The title is a lie.  JavaScript has no "that." We only have "this."

## The importance of ***this***

In object oriented programming "this" refers to the current argument.  It can be passed as an argument to a function.  In this case we are going to use + with a string to concatenate them.

```html
<h1 onmouseover="console.log('I am in ' + this)">Hello</h1>
<p onmouseover="console.log('In paragraph')" onmouseOut="console.log('Leaving Paragraph')">This is a paragraph</p>
```
## Functions

We have seen built-in functions console.log("some message") and alert("some message"). 

But we can write our own functions.  Normally these are placed in the &lt;head>.

In functions we write several commands together.

```html
<script>
  function poem(){
    console.log('There once was a lady from Bright');
    console.log('   whose speed was much faster than light.');
    console.log('She set off one day,');
    console.log('   in a relative way,');
    console.log('   and returned the previous night');
  }
</script>  
</head>
<body>
<button onclick="poem()">Click me and check the console.</button>
```
### Variables

Variables are words that we use to hold data.  The variable can be used to pass data around.

### Arguments and Parameters

For this class, we won't quibble about the distinction between arguments and parameters.

Parameters are inside the parenthesis of a function.  It is a local name to the function.

```html
<script>
  function makeHighlight(current){
    current.style.color = "blue";
    current.backgroundColor = "lightblue";
  }
  function unHighlight(me){
    me.style.color = "black";
    me.backgroundColor = "white";
  }
</script>
</head>
<body>
  <h1 id="geography" onmouseover="makeHighlight(this)" onmouseout="onmouseout">Peoria</h1>
  <section id="geography" onmouseover="makeHighlight(this)" onmouseout="onmouseout">
  <h2>Geography</h2>
    <p>Peoria is a city in roughly the center of Illinois</p>
  </section>
```

In the above code notice that the name of the argument is "this" in the html code.  But in the functions it is called "current" and "me" in the functions.  Actually, both functions could have used "current" or "me."  The parameter of a functon is local to that function.

We say that the value of the parameter is "passed" over to the function.  The value is passed.  The name may be different in differenct in different places.



