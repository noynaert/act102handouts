13e Variables

Variables store data temporarily.

There are a few pre-defined variables.  We have already seen "this" which refers to the current object.  But most of the time the programmer gets to make up a name.  There are rules that variable names must follow.

* The variable name must begin with a letter.
  * Technically, names may also begin with $ and _, but you should not do this.  Variables starting with _ or $ are often system-wide variables, and typical users should avoid them.
* After the first letter, the name may contains letters, digits, underscores, and $ signs.  But I suggest you avoid $ signs.
*Names are case sensitive.  "payRate" and "payrate" are different names.
*There are reserved words like "this" and "function" that may not be used.

In general, keep variable names simple and meaningful.  Start them with lowercase letters.  Blank spaces are not allowed in variable names.  If you want to use two words, run them together and capitalize them like ```payRate```.

## Declaring variables

There are several ways to declaring variables.  We will only use two of them in this course.

1. Use the variable name inside the () marks when declaring a function
2. Use the reserved word "var."

### Declared as the parameter to a function

```javascript
function add(first, second){
  console.log("First is "+ first);
  console.log(Second is "+ second)
}
```
In the above example the two variable names are "first" and "second."  They are only available within the function itself.

### Declared with ```var```

function add(first, second){
 var answer;
 answer = first + second;  //may hold a number
 console.log(answer);
 answer = "A String";     //may hold a string
 console.log(answer);
 answer = "45";     //may hold a number as a string
 console.log(answer);
 answer = new Date();  //may hold an object
 console.log(answer;)
}

### Variables may be declared and given a value in the same statement.

```javascript
function triple(number){
  var answer = number * 3;
  console.log(answer);
}
```

### Sometimes we do not even need to create a variable

```javascript
function printer(someId){
  console.log( 5 + 6 );
  console.log(document.getElementById('someId').innerHTML);
}
```

