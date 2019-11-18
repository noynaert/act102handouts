# 13b JavaScript Getting Started

## Open the Console!

Any time you are doing JavaScript, open the console!  Every time!

* Go into developer mode
    * The easiest way is usually to right-click on an element and then pick "Inspect" at the bottom of the list.
    * Move the developer window to the right if you have a wide screen, or to the bottom if your screen is narrow.
* Click on "Console"

## Where does Java go?

The ```<script>``` tag

*  Javascript may go inside the pair of ```<script>...</script>``` tags similar to the way ```<style>...</style>``` works
* You may include an external source file as ```<script src="something.js"></script>```

### Head or Body?

Placing JavaScript on your page can be tricky.

* Functions should go in the ```<head>```, but 
* The script may be in the body.  It is often placed at the end of the body.
* You may have more than one Script tag.

## Output

1. document.write("Hi, there");
2. console.log("Only the programmer is likely to see this");
3. alert("Did this message annoy you?")
4. Replacing items on the page.  This is the most common.  Remember "Manipulating the DOM"  This is what we will do most of the time.

## Strings

Strings may either be enclosed with 'single quotes' or "double quotes."

There is no difference between single quotes.  If your string contains an apostrophe, then use double quotes.  If your string includes quote marks, then use single quotes.  If it uses both an apostrophy and double quotes, then you probably need to use the html entities ```&apos;``` or ```&quot;```.

Strings may be concatinated with the &plus; symbol

```
console.log("How now " + "brown cow.")
)
```