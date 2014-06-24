JQuery Lesson Plan
==================

## FlickrMap Functions Used

* `$(document).ready`
* `$.getJSON`
* `$.each`
* `$(“#id”).append`

## Concepts

* [Javascript Libraries](#javascript-libraries)
* [Selectors](#selectors)
* [DOM Manipulation and Traversal](#dom-manipulation-and-traversal)

### Javascript Libraries

* How do we link in Javascript Files?  What does this really do?
* What is a coding library?  Why do we need it?
* Linking and JQuery Library?
* Show an example of some simple JQuery function.
* Make a note of minification.  See if we can show the same function minified?
* Hackers go to the [**Source**](https://github.com/jquery/jquery)
* Open vs Closed Source, why it's bad and why Javascript encourages open source.
* [API Reference](http://api.jquery.com/)

### [Selectors](http://api.jquery.com/category/selectors/)

* Basis of JQuery is easily selecting elements in the DOM and:
  + Performing some operation/modification to them
  + Reacting to some event (not necessarily user generated)
* First we’ll cover the basis of selectors with the $ sign, then tools to change them
* What is the DOM?  Show HTML and a *tree* and how the HTML maps to a tree structure.  Emphasize how it is a representation of the actual HTML and how it is possible to manipulate it with Code.
* So, what is this `$` thing really?  Alias for `JQuery`, which is really a function that takes one string argument.
  + [JQuery.fn.init](https://github.com/jquery/jquery/blob/master/src/core/init.js#L16)
* Examples
  + Any valid CSS selector - .class, #id, html
  + Multiple selectors - `$("select1,select2,selector3")`
  + Attribute values - `$("input[value='Hot Fuzz']").next().text("Hot Fuzz");`
  + Many more - http://api.jquery.com/category/selectors/

### DOM [Manipulation](http://api.jquery.com/category/manipulation/) and [Traversal](http://api.jquery.com/category/traversing/)

