# jQuery 

**jQuery offers a simple way to achieve a variety of common JavaScript tasks quickly and consistently, across all major browsers and without any fallback code needed.**

* SELECT ELEMENTS It is simpler to access elements using jQuery's CSS-style selectors than it is using DOM queries.The selectors are also more powerful and flexible.

* PERFORM TASKS:jQuery's methods let you update the DOM tree,animate elements into and out of view, and loop through a set of elements,all in one line of code.


* HANDLE EVENTS: jQuery includes methods that allow you to attach event listeners to selected elements without having to write any tailback code to support older browsers

## WHY USE JQUERY? 

**jQuery doesn't do anything you cannot achieve with pure JavaScript. It is just a JavaScript file but estimates show it has been used on over a quarter of the sites on the web, because it makes coding simpler.**

1: SIMPLE SELECTORS:

jQuery uses a language that is already familiar to front-end web developers: CSS selectors. They:

 • Are much faster at selecting elements 
 
 • Can be a lot more accurate about which elements to select 
 
 • Often require a lot less code than older DOM methods 
 
 • Are already used by most front-end developers 

**jQuery even adds some extra CSS-style selectors which offer additional functionality.**

2: COMMON TASKS IN LESS CODE:

**jQuery has methods that offer web developers simpler ways to perform common tasks, such as:**

• loop through elements

• Add I remove elements from the DOM tree

• Handle events

• Fade elements into I out of view 

• Handle Ajax requests 

**jQuery simplifies each of these tasks, and allows you to write less code to achieve them.**

3: CROSS-BROWSER COMPATIBILITY:

* jQuery automatically handles the inconsistent ways in which browsers select elements and handle events, so you do not need to write cross-browser fallback code 

## Amatches set/jquery selection


![img](/img/single.png)

![img](/img/set.png)

# LOOPING 

**In plain JavaScript, if you wanted to do the same thing to several elements, you would need to write code to loop through all of the elements you selected**

*With jQuery, when a selector returns multiple elements, you can update all of them using the one method. There is no need to use a loop*

## CHAINING

The process of placing several methods in the same selector is referred to as chaining


![img](/img/sentax.png)

# UPDATING ELEMENTS

Here are four methods that update the content of all elements in a jQuery selection :

* html() :

This method gives every element in the matched set the same new content. The new content may include HTML.

* text():

This method gives every element in the matched set the same new text content. Any markup would be shown as text. 

* replaceWith():

This method replaces every element in a matched set with new content. It also returns the replaced elements.

* remove():

This method removes all of the elements in the matched set. 

# INSERTING ELEMENTS 

Inserting new elements involves two steps:

 1: Create the new elements in a jQuery object 
 
 2: Use a method to insert the content into the page 

* before():

This method inserts content before the selected element(s) . 

* prepend():

This method inserts content inside the selected element(s), after the opening tag

* after():

This method inserts content after the selected element(s). 

* append():

This method inserts content inside the selected element(s), before the closing tag


# GETTING AND SETTING ATTRIBUTE VALUES 

.attr() 

This method can get or set a specified attribute and its value. To get the value of an attribute, you specify the name of the attribute in the parentheses. 

. removeAttr() 
This method removes a specified attribute (and its value). You just specify the name of the attribute that you want to remove from the element in the parentheses. 

. addCl ass() 

This method adds a new value to the existing value of the cl ass attribute. It does not overwrite existing values. 

.removeClass() 

This method removes a value from the cl ass attribute, leaving any other class names within that attribute intact. 
These 

# WHERE TO PLACE YOUR SCRIPTS

The position of <script> elements can affect how quickly a web page seems to load. 

* in the head

* in the page

* before the closing </body> tage

# Why pair program?

1. Greater efficiency

2. Engaged collaboration

3. Learning from fellow students

4. Social skills

5. Job interview readiness

6. Work environment readiness

# EFFECTS 

**When you start using jQuery, the effects methods can enhance your web page with transitions and movement.**

