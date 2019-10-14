# 09a Tables

## References

* Chapter 6 of the textbook
* [W3C for all versions of HTML](https://www.w3schools.com/html/html_tables.asp)
* [html5 &lt;thead>, &lt;tbody>, and &lt;tfoot> Tags](https://www.w3schools.com/tags/tag_thead.asp)

### Reference Videos

* [CSS Variables](https://mwsu.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=fcb5a4e4-1a20-4fe0-b605-aae5011db3f6) -- ***Guest video by Darth V.*** -- Apparently Darth was upset because I didn't show people Cascading variables before Homework 6.  So he contributed a video.
* [Basic Tables](https://mwsu.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=321adcb5-7119-4402-8318-aae6005c591e)
* [Head and Captions](https://mwsu.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=7a524cc2-dc99-4fe1-97a8-aae6005c58d4)
* [thead, tbody, tfoot](https://mwsu.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=321adcb5-7119-4402-8318-aae6005c591e)

## Basic Tables in all Versions of HTML

[Video for Basic Tables](https://mwsu.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=321adcb5-7119-4402-8318-aae6005c591e)

```html
    <table>
        <!-- This is the head (or top row with labels) -->
        <tr>
            <td>State</td><td>Capital</td><td>Population</td><td>Flag</td>
        </tr>
        <!-- Body of the table-->
        <tr>
           <td>Missouri</td>
           <td>Jefferson City</td>
           <td>6,113,532</td>
           <td><img src="images/125px-Flag_of_Missouri.svg.png"alt="Flag of Missouri"></td>
        </tr>
        <tr>
                <td>Iowa</td>
                <td>Iowa City</td>
                <td>3,145,711</td>
                <td><img src="images/125px-Flag_of_Iowa.svg.png"alt="Flag of Iowa"></td>
        </tr>
        <!-- This is the footer at the bottom of the table-->
        <tr>
            <td colspan="4">Total Population: 24974389</td>
        </tr>
    </table>
```

### Basic Tags

* ***&lt;table>*** Surrounds the entire table, including the caption
* ***&lt;tr>*** Defines one row of the table
* ***&lt;td>*** Defines one cell.  Always appears inside a &lt;tr> tag
* ***&lt;th>*** Defines one cell *in the top row*.  Always appears inside a &lt;tr> tag
* ***&lt;caption>*** Optionally provides a caption

### Spanning rows and columns

If you want to combine rows or columns, use the following properties

* colspan="2" This would span 2 cells horizontally.  You may span any positive number of columns
* rowspan="2" This combines cells vertically  You may span any positive number of rows.

## Cell content

Cell content may include almost anything that would go in a paragraph.  This includes images, lists, and links.

## CSS for tables

Usually you specify a rule like this for the table.

```css
table, tr, td {border:1px solid black;
               border-collapse:separate;
}
```
Note the commas in ```table,tr,td``` 

The borders are handy for debugging.  If you do not want them to show in your final product change the color of the border to the background color of the page (usually white).

Padding and borders may be applied to cells, but not margins.

## The Head and Caption

[Video for Head and Captions](https://mwsu.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=7a524cc2-dc99-4fe1-97a8-aae6005c58d4)

### CSS for captions

Captions are optional.  You could specify them something like the following.  Note that ```table caption``` does *not* have a comma.  This means "caption which is inside a table."  

```css
table caption {font-size:200%;
               font-weight:bold;
}
```

## HTML5 tags

[Video for thead, tbody, tfoot](https://mwsu.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=321adcb5-7119-4402-8318-aae6005c591e)

Html5 introduced the following tags.  You should always use them in your tables.  Older browsers will just ignore them.  

* &lt;thead>
* &lt;tbody>
* &lt;tfoot>

Using the tags gives you some html styling options.  They are also important for packages like Bootstrap.  Using the tags also helps search engines and other AI programs analyze the data on your page.