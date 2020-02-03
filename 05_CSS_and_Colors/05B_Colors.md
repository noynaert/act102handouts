# Colors

## Color Names

Modern browsers support 140 color names.  

See https://htmlcolorcodes.com/color-names/ for a list of names.

## Mixing Colors

There are two sets of rules for mixing colors.

* Mixing pigments (like paint)
* Mixing light (what we will be concerned with)

### Mixing pigments

In grade school you learned the primary colors are Red, Yellow, and Blue.  But these are the primary colors when mixing pigments such as paint.  We don't care about those colors in this class.

### Mixing light

When mixing light the primary colors are:

* Red
* Green
* Blue

![RGB Colors Demo](images/rgb.gif)

The order is important because of the way we code the colors.

There are a lot of different coding systems for specifying colors.  For web pages we usually use RGB colors.  RGB stands for "Red Green Blue."  The order is important.

Each of the RGB colors is represented by a number from 0 through 255.  0 represents none of the color (that color is turned off).  255 represents all of the color available.

We are dealing with 8 bit numbers.  2<sup>8</sup> is 256.  We use 0 through 255 which is 256 different intensities of color.

* Pure red would be 255, 0, 0
* Pure green would be 0, 255, 0
* Pure blue would be 0, 0  255
* What color would 255, 255, 0 be?
* What color would be 255, 0, 255 be?
* What color would 255, 255, 255 be? (turn on all the lights)
* What color would 0, 0, 0 be? (turn off all the lights)
* What color would 127, 127, 127 be?

#### Hexadecimal

Hex or hexadecimal is shorthand for writing numbers.  It is ideally suited to representing numbers that are 8 bits.  You don't have to be able to do all of the number of conversions, but you should be able to approximate magnitude (in other words, tell whether a hexadecimal number is near zero, in the middle, or near 255).  Here are some examples to give you an idea.
|Decimal | Hex
:---:|:---:
0|00
65|41
127|7F
128|80
192|C0
255|FF

If you need more than a rough guess, Windows calculator will do conversions between hex and decimal.

### RGB Notation

Think of three lights that are red, green, and blue.  Each light has a dimmer switch that can go from 0 to 255 (or 0 to FF).  0 is off and FF is all the way on.  Something like 80 is half way on.  (we can use upper or lower case)

* #FF0000 is red
* #00FF00 is green
* #0000FF is blue
* #FFFFFF is white (all lights on full blast)
* #000000 is black (all the lights off)

All these would be grey.  Which would be light grey and which would be dark grey?

* #111111
* #888888
* #cccccc

Now look at the [color names page](https://htmlcolorcodes.com/color-names/) page again.  Look at Indiared which has a color of #CD5C5C. Compare the red value of CD with the green and blue colors of 5C and 5C.  By inspecting the code you can tell it is "more red with sort of low amounts of green and blue."

* Is #E6E6FA going to be a very light or a very dark color?  Which color is going to be the strongest?
* What can you say about #ADFF2F just by looking at the RGB?
* What do you think the name of #FF6347 is?  Here are your choices:
  * Banana
  * Blueberry
  * Tomato
  * Cucumber

## Color in CSS

```css
h1 {color: #FF0000;
    background-color: #555555;
   }
```

## Other colors to know

If you are dealing with colors you need to know a couple of other color names as well:

* Cyan : Green + Blue (no red)
* Magenta: Red + Blue (no green)
* Yellow: Red + Green (no blue)

## Notes about the color-mixing image

I made the image using https://www.kapwing.com/ from youtube video https://www.youtube.com/watch?v=xzmXrC-Yzfc .  I saved to GIF format, so depending on your monitor or display there may be some odd artifacts in the image.  We will talk about why that is happening in the unit on images.
