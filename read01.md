# Responsive Web Design

## Responsive Overview

**Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.**

## Responsive vs. Adaptive vs. Mobile

*Responsive generally means to react quickly and positively to any change*

*Adaptive means to be easily modified for a new purpose or situation, such as change*

*Mobile means to build a separate website commonly on a new domain solely for mobile users.*

# Responsive web design is broken down into three main components, including:

## Flexible Layouts:

 *flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. Flexible grids are built using relative length units, most commonly percentages or em units. These relative lengths are then used to declare common grid property values such as width, margin, or padding.*

 *Flexible layouts do not advocate the use of fixed measurement units, such as pixels or inches. Reason being, the viewport height and width continually change from device to device. Website layouts need to adapt to this change and fixed values have too many constraints*

 **The formula is based around taking the target width of an element and dividing it by the width of it’s parent element. The result is the relative width of the target element.**

 * target ÷ context = result

## Flexible Grid:

*Let’s see how this formula works inside of a two column layout. Below we have a parent division with the class of container wrapping both the section and aside elements. The goal is to have have the section on the left and the aside on the right, with equal margins between the two.*

**HTML**

**<div class="container">**

 **<section>...</section>**

  **<aside>...</aside>**
  
**</div>**

**CSS**

**.container {**

  **width: 538px;**

**}**

**section,**

**aside {**

 **margin: 10px;**

**}**

**section {**

  **float: left;**

  **width: 340px;**
**}**

**aside {**

  **float: right;**

  **width: 158px;**

**}**

**section,**

**aside {**

  **margin: 1.858736059%; /*  10px ÷ 538px = .018587361 */**

**}**

**section {**

  **float: left;**

  **width: 63.197026%;    /* 340px ÷ 538px = .63197026 */** 

**}**

**aside {**

  **float: right;**

  **width: 29.3680297%;  /* 158px ÷ 538px = .293680297 */**

**}**

## Media Queries

**Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation**

## Media Features in Media Queries

*Media features identify what attributes or properties will be targeted within the media query expression*

## Viewport#viewport

**Mobile devices generally do a pretty decent job of displaying websites these days. Sometimes they could use a little assistance though, particularly around identifying the viewport size, scale, and resolution of a website. To remedy this, Apple invented the viewport meta tag.**

## Flexible Media

**The final, equally important aspect to responsive web design involves flexible media. As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.**


# What is "Float"?

**Float is a CSS positioning property**

*There are four valid values for the float property. Left and Right float elements those directions respectively. None (the default) ensures the element will not float and Inherit which will assume the float value from that elements parent element.*

**What are floats used for?**

**Aside from the simple example of wrapping text around images, floats can be used to create entire web layouts.**

![img](https://i1.wp.com/css-tricks.com/wp-content/csstricks-uploads/web-layout.png?resize=540%2C240&ssl=1)

*Floats are also helpful for layout in smaller instances. Take for example this little area of a web page. If we use float for our little avatar image, when that image changes size the text in the box will reflow to accommodate:*

![img](/img/reflow-example-1.png)

*This same layout could be accomplished using relative positioning on container and absolute positioning on the avatar as well. In doing it this way, the text would be unaffected by the avatar and not be able to reflow on a size change.*

![img](/img/reflow-example-2.png)

**Clearing the Float**

**Float's sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float. Again an illustration probably does more good than words do.**

![img](/img/unclearedfooter.png)


**In the above example, the sidebar is floated to the right and is shorter than the main content area.**

*The footer then is required to jump up into that available space as is required by the float. To fix this problem, the footer can be cleared to ensure it stays beneath both floated columns.*

**#footer {**

  **clear: both;**

**}**

![img](/img/clearedfooter.png)

**clear has four valid values as well. Both is most commonly used, which clears floats coming from either direction. Left and Right can be used to only clear the float from one direction respectively. None is the default, which is typically unnecessary unless removing a clear value from a cascade. Inherit would be the fifth, but is strangely not supported in Internet Explorer. Clearing only the left or right float, while less commonly seen in the wild, definitely has its uses.**

![img](/img/directionalclearing.png)




# Don’t Overthink It Grids

## Context

**A block level element is as wide as the parent it's inside (width: auto;). We can think of it as 100% wide. The wrapper for a grid probably don't have much to do with semantics, it's just a generic wrapper, so a div is fine.**

**<div class="grid">**

  **<!-- 100% wide -->**

**</div>**


# grid context

## Columns

*Let's start with a practical and common need: a main content area being 2/3 the width and a sidebar being 1/3 the width. We just make two column divs with appropriate class names.*

[img](/img/grid.png)

[img](/img/grid2.png)


## Clearing Context

**The parent element will collapse to zero height since it has only floated children. Let's fix that by clearing it. These days all you need is this:**

**.grid:after {**

  **content: "";**

  **display: table;**

  **clear: both;**

**}**

## Gutters

**The hardest part about grids is gutters. So far we've made our grid flexible by using percentages for widths.**

* The first step toward this is using box-sizing: border-box;

[img](/img/grid3.png)

* The second step is applying a fixed padding to the right side of all columns except the last one.

[img](/img/grid4.png)


# CSS Floats Explained By Riding An Escalator

## Floats: Left and Right

* Using floats can introduce up to two new flows: left and right.

* And this allows the normal flow of elements, those without a float value, to fill in the spaces around these elements

* Floats allow you to create these new relationships between flows.


# SMACSS Official Documentation

# What is it?

**SMACSS is a way to examine your design process and as a way to fit those rigid frameworks into a flexible thought process. It is an attempt to document a consistent approach to site development when using CSS.**

**At the very core of SMACSS is categorization. By categorizing CSS rules, we begin to see patterns and can define better practices around each of these patterns.**

**There are five types of categories:**

* Base: Base rules are the defaults. They are almost exclusively single element selectors but it could include attribute selectors, pseudo-class selectors, child selectors or sibling selectors.

* Layout: divide the page into sections. Layouts hold one or more modules together.

* Module: are the reusable, modular parts of our design. They are the callouts, the sidebar sections, the product lists and so on.

* State: are ways to describe how our modules or layouts will look when in a particular state. Is it hidden or expanded? Is it active or inactive? They are about describing how a module or layout looks on screens that are smaller or bigger. They are also about describing how a module might look in different views like the home page or the inside page.

* Theme: are similar to state rules in that they describe how modules or layouts might look. Most sites don’t require a layer of theming but it is good to be aware of it.

