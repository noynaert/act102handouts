## 07_40 CSS Variables

CSS variables make it easier to maintain consistency across a website.

CSS variables may be declared with any CSS selector.  However, often we want the variable to apply
to all scopes.  Therefore the scope is often defined as ```:root``` so that it has global scope.

## Declaring Variables

```css
   :root {--primaryColor: #0000ff;
          --accentColor:  #ff4500;
          --borderFormat: 1px solid var(--accentColor);
          --defaultImgWidth: 250px;
          --defaultImgHeight: 250px;
   }

## Using Variables

   .productSidebar {color: var(--primaryColor);
                    background-color: var(--accentColor);
                    border: var(--borderFormat);
   }
```

## Variables and the Cascade

The CSS Cascade rules still apply to variables.

Often a file containing variables needs to be applied across other stylesheets.  Therefore a file containing the variable declarations often is placed first.

In the case of Homework 7, we put the variable file last because we wanted to overrule any styling that was in the layout or footer.  In a larger application we probably would have split the color harmony file into two parts.  The first part would have defined the variables, and it would have been placed first.  A second file that used the variables would have been placed last.
