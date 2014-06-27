JQuery Lesson Plan
==================

Ideas and notes for ScriptEd Bootcamp Lesson.  First I'll list out objectives, then an outline of topics to be 
discussed to meet those objects.  Also included are a list of JQuery functions used in FlickrMap project and exercises
for students to practice JQuery skills. I won't necessarily cover every function listed as examples, these are just
a pool to draw from to do live coding examples with the students.

# Content

* [Javascript Libraries](#javascript-libraries)
* [Selectors](#selectors)
* [DOM Manipulation and Traversal](#dom-manipulation-and-traversal)
* [Events](#events)
* [FlickrMap](#flickrmap)

## Javascript Libraries

### Goals

* Understand how Javascript libraries are linked together.
* Comprehend the concept of a *dependency* and how libraries are related.
* Analyze why JQuery is considered a library and the function it serves.
* Understand how to look at library source code.
* Be able give examples of other possible Javascript Libraries.

### Outline

* How do we link in Javascript Files?  What does this really do?
* What is a coding library?  Why do we need it?
* Linking and JQuery Library?
* Show an example of some simple JQuery function.
* Make a note of minification.  See if we can show the same function minified?
* Hackers go to the [**Source**](https://github.com/jquery/jquery)
* Open vs Closed Source, why it's bad and why Javascript encourages open source.
* [API Reference](http://api.jquery.com/)

## [Selectors](http://api.jquery.com/category/selectors/)

### Goals

* Compare and contrast JQuery and CSS selectors.
* Explain how the DOM is like a tree.
* Take a simple HTML page and draw out the DOM.
* Explain what the `$` in JQuery is.
* Given an arbritrary HTML be able to use selectors to navigate to any element.

### Outline

* Basis of JQuery is easily selecting elements in the DOM and:
  + Performing some operation/modification to them
  + Reacting to some event (not necessarily user generated)
* First we’ll cover the basis of selectors with the $ sign, then tools to change them
* What is the DOM?  Show HTML and a *tree* and how the HTML maps to a tree structure.  Emphasize how it is a representation of the actual HTML and how it is possible to manipulate it with Code.
* So, what is this `$` thing really?  Alias for `JQuery`, which is really a function that takes one string argument.
  + [JQuery.fn.init](https://github.com/jquery/jquery/blob/master/src/core/init.js#L16)
* Examples
  + Any valid CSS selector - `.class`, `#id`, `html`
  + Multiple selectors - `$("select1,select2,selector3")`
  + Attribute values - `$("input[value='Hot Fuzz']").next().text("Hot Fuzz");`
  + Many more - http://api.jquery.com/category/selectors/

## DOM [Manipulation](http://api.jquery.com/category/manipulation/) and [Traversal](http://api.jquery.com/category/traversing/)

### Goals

* Describe inserting into and modifying nodes in the DOM tree.
* Use JQuery to modify all aspects of HTML on a page.

### Outline

* Illustrate how you might insert objects into a tree.
* Tie back to examples of inserting new DOM elements with JQuery
  + `.append()`, `.prepend()`, `.html()`, and `.text()`
  + `after()` and `before()`
  + `empty()` and `remove()`
* Now discuss modifiying a tree.
* Again, tie back with examples in JQuery with the DOM
  + `attr()`, `removeAttr()`, `prop()`, and `removeProp()`
  + `val()`
  + `addClass()`, `hasClass()`, `removeClass()`
  + `css()`, `width()`, `height()`
  
## [Events](http://api.jquery.com/category/events/)

### Goals

* Summarize what it means to be *Event Driven*.
* Describe how *Event Driven* programming is different from *Procedural*.
* Name the source of events on a web page.
* Describe what Javascript functions have to do with events.
* Be able to write sample code that reacts to several different types of events and manipulates the DOM in some way
based off those events.

### Outline

* In everday terms what is an event?  How do you plan your day?  Do you do everything as it comes to your mind at that
very moment, or do you plan out times and places to meet people, do errands, etc?
* Just like you have a Calendar a computer can have one as well and it doesn't have to do something the exact moment you
tell it to.  It can either run it at some random time in the future or some other action (i.e., by a human) can cause
it to do something.
* Programming like this is called *Event Driven*, whereas having a computer do everything right when you code it is
called *Procedural*.
* Javasscript and JQuery rely very heavily on event driven designs.
* Examples to go over in JQuery:
  + `click()` and `dblclick()`
  + `hover()` and `focus()`
  + `keypress()` and `mousedown()`
  + `on()`, `submit()`, and `ready()`
  

## Exercise

During the lesson we will go over a sample app that allows you to pick the winning countries in the World Cup final round of 16.  We use javascript to make an interactive bracket adding country selection and a form to dynamically change countries that are in the bracket.

### Extra Exercises

* Change text and background color for each country through the form.
* Add images of country flags through the form.
* Label games, i.e. 'Round of 16', 'Quarter Finals', etc. Make sure they change correctly as different games take place.
* When a country wins a final have a celebratory gif pop up.
* Improve bracket design anyway you can think of.
* Fix final country over riding form when you click on it again.

## FlickrMap 

### Functions Used

* `$(document).ready`
* `$.getJSON`
* `$.each`
* `$(“#id”).append`
