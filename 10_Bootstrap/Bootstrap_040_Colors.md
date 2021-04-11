# Bootstrap 030 Colors

You may use colors as you choose, but Bootstrap encourages "meaning through colors."  The idea is that meanings are assigned to colors, and when people
see those colors they get meaning from the color itself.  For example, the -warn colors are red, and the -success colors are green.

I think "meaning through colors" was a good idea.  It does have some problems.  One of the big criticisms is actually a legal criticism in the US.  When you try to convey
meaning through colors you run into ADA (Americans with Disability Act) problems.  The original intent with Bootstrap was that screen readers would be adapted to actually
read the bootstrap warning colors, but this did not pan out.  And screen readers do not address some other ADA issues such as color blindness.  Another problem is that the
meanings don't always work for websites.

What I have seen is a lot of sites just using the bootstrap colors for a general color palette.  They aren't too bad as a color palette.  They are basically a pastel color
palette with a modern feel.  It is possible to do warm, cool, neutral, and even monochromatic themes, especially if you use SASS.  SASS is a tool used very commonly in the industry, but we will not cover it in this unit.

## Standard Foreground Colors:

* .text-muted
* .text-primary
* .text-success
* .text-info, .text-warning
* .text-danger 
* .text-secondary 
* .text-white 
* .text-dark 
* .text-body (default body color/often black)
* .text-light

## Standard Background Colors:

* .bg-primary
* .bg-success
* .bg-info
* .bg-warning
* .bg-danger
* .bg-secondary
* .bg-dark 
* .bg-light

[Illustration of the colors](https://getbootstrap.com/docs/4.5/utilities/colors/)

## Doing other colors

### Method 1: SASS

SASS is an alternative method of creating CSS.  If you follow the [Illustration of the colors](https://getbootstrap.com/docs/4.5/utilities/colors/) link you will see that
at the bottom they say to use SASS if you want to enable gradients.

SASS colors beyond the standard text- and bg- colors are mostly enabled using SASS.  You may also use SASS change the basic colors assigned to the standard bootstrap colors palette.

[This page](https://getbootstrap.com/docs/5.0/customize/color/) gives a much more in-depth look at colors. I suggest that you take a look, even though we are not doing SASS here.  Scroll down the page and notice their color system.  Look at how the color $blue is done.  (The $ indicates a SASS variable, similar to -- in CSS variables).  Note that they use
a scale of -100 through -900.  This is the same scale that is used in CSS for font-weight, or boldness.  Together SASS and Bootstrap let you just set pick a color and set the
value of the -500 level.  SASS and Bootstrap then automatically calculate all of the other colors.

### Method 2: Plain old .css

We can still use CSS with Bootstrap.  In fact, most big sites that use Bootstrap also use CSS.  We need to be careful to place our own CSS *after* our link to Bootstrap.  This is why I like to put the link to bootstrap above the &lt;title> and the link to the local CSS file below the &lt;title>

Define variables and classes.  Give the classes names similar to what Bootstrap would use, but put something like your initials or some other unique sequence in front of them so they are not confusing to you or other developers who come after you.

```css
    :root {
        --orange: #fd7e14;
        --indigo: #6610f2;
      }

    .jen-text-indigo   { color: var(--indigo);}
    .jen-bg-indigo     { background-color: var(--indigo);}
    .jen-border-indigo {border-color: var(--indigo);}
```

