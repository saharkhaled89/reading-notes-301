# Javascript Templating Language and Engine— Mustache.js with Node and Express

## Javascript Templating

**Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic.**

**The template engine then replaces variables and instances declared in a template file with actual values at runtime, and convert the template into an HTML file sent to the client.**

# Mustache

*Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.*

![img](/img/ma.png)

# A Guide to Flexbox

![img](https://css-tricks.com/wp-content/uploads/2018/10/01-container.svg)

# display

*This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.*

*.container {*
  *display: flex; /* or inline-flex */*
}
*Note that CSS columns have no effect on a flex container.*


![img](/img/flex.png)


![img](/img/02-items.svg)


![img](/img/p.svg)


* flex-start / start: items packed to the start of the container. The (more supported) flex-start honors the flex-direction while start honors the writing-mode direction.

* flex-end / end: items packed to the end of the container. The (more support) flex-end honors the flex-direction while end honors the writing-mode direction.

* center: items centered in the container

* space-between: items evenly distributed; the first line is at the start of the container while the last one is at the end

* space-around: items evenly distributed with equal space around each line

* space-evenly: items are evenly distributed with equal space around them

* stretch (default): lines stretch to take up the remaining space


# FLEXBOX FROGGY

* flex-start: Items align to the left side of the container.

* flex-end: Items align to the right side of the container.

* center: Items align at the center of the container.

* space-between: Items display with equal spacing between them.

* space-around: Items display with equal spacing around them.



# Use justify-content again to help these frogs get to their lilypads. Remember that this CSS property aligns items horizontally and accepts the following values:

* flex-start: Items align to the left side of the container.

* flex-end: Items align to the right side of the container.

* center: Items align at the center of the container.

* space-between: Items display with equal spacing between them.

* space-around: Items display with equal spacing around them.

# Now use align-items to help the frogs get to the bottom of the pond. This CSS property aligns items vertically and accepts the following values:

* flex-start: Items align to the top of the container.

* flex-end: Items align to the bottom of the container.

* center: Items align at the vertical center of the container.

* baseline: Items display at the baseline of the container.

* stretch: Items are stretched to fit the container.

# flex-wrap property, which accepts the following values:

* nowrap: Every item is fit to a single line.

* wrap: Items wrap around to additional lines.

* wrap-reverse: Items wrap around to additional lines in reverse.