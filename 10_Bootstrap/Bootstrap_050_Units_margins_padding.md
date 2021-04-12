# 10.050 Units, Margins, Padding, and Borders

## ```em``` vs ```rem```

* ```em``` is the size of a box that fits around the capital letter M in the ***current*** font
* ```rem``` is the size of a box that fits around the capital letter M in the ***root*** font of the viewport

Therefore ```em``` changes based on whether it is used in an &lt;h1> or an &ltp>.  ```rem``` will be a constant size across the whole page

## Margins and Padding

Margins and padding use the same system.  Margins are indicated by class names starting with m, and padding with class names starting with p.

### Sides

Sides are indicated by adding a character after the ```m``` or ```p```.  For example, ```mt``` sets the margin across the top.

* ```t``` - for classes that set margin-top or padding-top
* ```b``` - for classes that set margin-bottom or padding-bottom
* ```l``` - for classes that set margin-left or padding-left
* ```r``` - for classes that set margin-right or padding-right
* ```x``` - for classes that set *  ```both`` *-left and *-right
* ```y``` - for classes that set both *-top and *-bottom
* ```blank``` - for classes that set a margin or padding on all 4 sides of the element

### Sizes

Sizes are measured in ```rem```.

Size | Meaning
:-:|:--
0 | 0rem, no margin
1 | 0.25rem
2 | 0.50rem
3 | 1.00rem (This is the default if no size is specified)
4 | 1.50rem
5 | 3.00rem

If you need mixed sizes, list the most general first, and put the side designations after it.  For example, if you want padding of p-2 on three sides, but p-4 on top, use  ```class="p-2 pt-4"```

## Screen sizes

Several features of Bootstrap reference screen size.  This allows the developer to adapt how the formatting will look on different screen widths.  

### Standard Bootstrap Display Widths (Breakpoints)

| Breakpoint | Infix | Dimensions |
| :---:         |     :---:      | :--- |
| X-Small   | *None* | &lt;576px    |
| Small     | `sm`       | &ge;576px      |
| Medium     | `md`       | &ge;768px      |
| Large     | `lg`       | &ge;992px      |
| Extra Large     | `xl`       | &ge;1200px      |
| Extra extra Large     | `xxl`       | &ge;576px      |

Bootstrap uses the principle of "mobile first."  This generally means smaller screen sizes apply to everything larger as well as the specified size.  Examples:

* `class="p-2"` refers to small phones and everything larger.
* `class="p-md-3"` or `class="p-md"` would apply to Medium and larger screens, and there would be padding for X-Small and Small displays.
* `class="p-0 p-sm-1 p-md-2 p-lg p-xl-4 p-xl-5` would apply progressively larger padding as display sizes increase

## Borders and Rounded classes

[[See this page for Borders and Rounded classes]](https://getbootstrap.com/docs/5.0/utilities/borders/)  You should be able to deal with the official documentation at this point.  Also, note that the system is fairly predictable.  Between the predictability and Emmett, you don't have to memorize a lot in order to use Bootstrap.

Don't worry about the material below the SASS heading.  At least for this week.

Take note that many of the commands require you to have the `border` class before you can add other border features.  This is very similar to how tables work.

Take special note of the `rounded-pill` style

## Width

In its simplest form, width is specified in percentage.  It is based on the size of the container.

Allowable values are w-25, w-50, w-75, w-100, w-auto

Further specialization is possible using SASS.
