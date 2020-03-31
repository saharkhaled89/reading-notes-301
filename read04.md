# GRID

**when grid-column-start is used alone, the grid item by default will span exactly one column. However, you can extend the item across multiple columns by adding the grid-column-end property.**

**When pairing grid-column-start and grid-column-end, you might assume that the end value has to be greater than the start value. But this turns out not the case!**

**If grid items aren't explicitly placed with grid-area, grid-column, grid-row, etc., they are automatically placed according to their order in the source code. We can override this using the order property, which is one of the advantages of grid over table-based layout.**

**By default, all grid items have an order of 0, but this can be set to any positive or negative value, similar to z-index.**

**grid-template is a shorthand property that combines grid-template-rows and grid-template-columns.**

# Regex Tutorial

## Flags


**A regex usually comes within this form /abc/, where the search pattern is delimited by two slash characters /. At the end we can specify a flag with these values (we can also combine them each other):**

* g (global) does not return after the first match, restarting the subsequent searches from the end of the previous match

* m (multi-line) when enabled ^ and $ will match the start and end of a line, instead of the whole string

* i (insensitive) makes the whole expression case-insensitive (for instance /aBc/i would match AbC)


*Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern (i.e. a specific sequence of ASCII or unicode characters).*

*Fields of application range from validation to parsing/replacing strings, passing through translating data to other formats and web scraping.*

* data validation (for example check if a time string i well-formed)

* data scraping (especially web scraping, find all pages that contain a certain set of words eventually in a specific order)

* data wrangling (transform data from “raw” to another format)

* string parsing (for example catch all URL GET parameters, capture text inside a set of parenthesis)

* string replacement (for example, even during a code session using a common IDE to translate a Java or C# class in the respective JSON object — replace “;” with “,” make it lowercase, avoid type declaration, etc.)

* syntax highlightning, file renaming, packet sniffing and many other applications involving strings (where data need not be textual)


# Properties for the Parent

## (Grid Container)

display
Defines the element as a grid container and establishes a new grid formatting context for its contents.

Values:

* grid – generates a block-level grid

* inline-grid – generates an inline-level grid

**.container {**

**display: grid | inline-grid;**

**}**

# Properties for the Children**

## (Grid Items)

grid-column-start
grid-column-end
grid-row-start
grid-row-end

**Determines a grid item’s location within the grid by referring to specific grid lines. grid-column-start/grid-row-start is the line where the item begins, and grid-column-end/grid-row-end is the line where the item ends.**

Values:

* <line> – can be a number to refer to a numbered grid line, or a name to refer to a named grid line

* span <number> – the item will span across the provided number of grid tracks

* span <name> – the item will span across until it hits the next line with the provided name

* auto – indicates auto-placement, an automatic span, or a default span of one

# place-items

**place-items sets both the align-items and justify-items properties in a single declaration.**

**Values:**

*<align-items> / <justify-items> – The first value sets align-items, the second value justify-items. If the second value is omitted, the first value is assigned to both properties.*

**All major browsers except Edge support the place-items shorthand property.**

**For more details, see align-items and justify-items.**

# justify-content

**Sometimes the total size of your grid might be less than the size of its grid container. This could happen if all of your grid items are sized with non-flexible units like px. In this case you can set the alignment of the grid within the grid container. This property aligns the grid along the inline (row) axis (as opposed to align-content which aligns the grid along the block (column) axis).**

# align-content

*Sometimes the total size of your grid might be less than the size of its grid container. This could happen if all of your grid items are sized with non-flexible units like px. In this case you can set the alignment of the grid within the grid container. This property aligns the grid along the block (column) axis (as opposed to justify-content which aligns the grid along the inline (row) axis).*

# grid

**A shorthand for setting all of the following properties in a single declaration: grid-template-rows, grid-template-columns, grid-template-areas, grid-auto-rows, grid-auto-columns, and grid-auto-flow (Note: You can only specify the explicit or the implicit grid properties in a single grid declaration).**

**Values:**

 **none – sets all sub-properties to their initial values.**

 **<grid-template> – works the same as the grid-template shorthand.**

# Common Responsive Layouts with CSS Grid 

 **In the same way that flexbox gave us a way to layout block elements next to each other, CSS grid lets us not only arrange elements in a row or a column, but in multiple rows and columns. Finally two dimensional layouts are becoming simpler!**

## Large Image followed by articles

 ![img](/img/cat.gif)

 **This is a responsive template that you’ll see all over the web, a large intro image followed by smaller images, buttons or articles. Have a look at the code from the glitch link above.**

**The smaller images (in a grid!) are in the perfect layout to get you started with CSS grid. Grid gives us control over how wide or narrow each of the ‘grid cells’ get. This allows us to maintain a sensible aspect ratio to their height. In this example I’ve used:**

**grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));**


The Full Page Image Gallery

 ![img](/img/cat2.gif)

**This image gallery layout uses features of CSS grid to create different sizes of grid cells. I’ve used the span value on grid-columnand grid-row to make individual cells stretch over two or more slots in the track.

 *The line grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;*

*will create a grid with 6 columns which are each one fraction unit wide.They each share 1/6 of the width of the container.You could also use*
*grid-template-columns: repeat(6, 1fr);*

**to get the same result. Using the span value with a number will make a grid cell span that many rows, or columns . grid-column: span 2; for example, will create a cell that is two columns wide. I’ve used object-fit again to make the images keep their aspect ratio while filling the space of their containers. If the images in your gallery have more constraints than cat pictures, with regards to the space they’ll fit in then you can use media queries to change the number of rows or columns they span at different widths.**



