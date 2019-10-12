## 07aa CSS Variables

This material will not be on this exam.  I am putting this here as a reference for Fall, 2019 students.  It will not be on the Fall 2019 exam 2.

It is also here to remind me to add it to tested content beginning Spring, 2020 course

```css
   :root {--primaryColor: blue;
          --accentColor:pink;
          --borderFormat: 1px solid var(--primaryColor);
          --defaultImgWidth: 250px;
          --defaultImgHeight: 250px;
   }

   .productSidebar {color: var(--primaryColor);
                    background-color: var(--accentColor);
                    border: var(--borderFormat);
   }

```
