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

![img](img/web-layout(1).png)

*Floats are also helpful for layout in smaller instances. Take for example this little area of a web page. If we use float for our little avatar image, when that image changes size the text in the box will reflow to accommodate:*

![img](reflow-example-1.png)

*This same layout could be accomplished using relative positioning on container and absolute positioning on the avatar as well. In doing it this way, the text would be unaffected by the avatar and not be able to reflow on a size change.*

![img](reflow-example-2.png)

**Clearing the Float**

**Float's sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float. Again an illustration probably does more good than words do.**

![img](unclearedfooter.png)


**In the above example, the sidebar is floated to the right and is shorter than the main content area.**

*The footer then is required to jump up into that available space as is required by the float. To fix this problem, the footer can be cleared to ensure it stays beneath both floated columns.*

**#footer {**

  **clear: both;**

**}**

![img](clearedfooter.png)

**clear has four valid values as well. Both is most commonly used, which clears floats coming from either direction. Left and Right can be used to only clear the float from one direction respectively. None is the default, which is typically unnecessary unless removing a clear value from a cascade. Inherit would be the fifth, but is strangely not supported in Internet Explorer. Clearing only the left or right float, while less commonly seen in the wild, definitely has its uses.**

![img](directionalclearing.png)

