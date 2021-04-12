# Bootstrap 10.060 Grid

## References

* [https://getbootstrap.com/docs/5.0/layout/grid/](https://getbootstrap.com/docs/5.0/layout/grid/)
* https://www.w3schools.com/bootstrap/bootstrap_grid_system.asp

## Uses

* Layout
* Alternative (more powerful) version of flexboxes
* Alternative to tables

## The Grid System

The Bootstrap grid system is based on there being 12 "spans."

### Why 12?

12 is evenly divisible by 1, 2, 3, 4, 6

### container

The grid *must* be in a `container` or a `container-fluid` (container-fluid takes up the maximum width)

If you don't specify how wide each column will be, each column is the same width.

## Controlling Display property

In regular css we covered display.  
* display:none
* display:block
* display:inline
* display:flex

These have the equivalent bootstrap.  But they are tied to size, so we can change the display property based on screen size.

This is useful for making decorative or less-needed material on small screens.  For example, you might have a sidebar that shows up on desktops, but not on small screens.  

The following code would make the image go to display:none on extra-small and small screens, but it would appear on medium and larger displays

```html
<div class="w-25 float-start d-none d-md-block">      
  <img class="w-100"src="images/NewTux.svg" alt="Tux, the Linux Mascot" />
</div>
```
### Controlling Printing

It is also possible to make things appear or disappear when a page is printed.  It works just like display, but with "print" where the size would go.

To make an item disappear on print do `class="d-print-none"`

To make an item appear on print, but not display on the screen do `class="d-print-block d-none"`
