# JavaScript Basics

This is a series of very simple examples for learning some JavaScript basics.

## Tools

Some essential tools (all free) you should have installed:

* **Visual Studio Code** - Probably the best development editor for many languages, especially for Java Script: [Website with download link](https://code.visualstudio.com/)
* **Git** - Version Control System to keep track of changes and manage variants of your code: [Website with download link](https://git-scm.com/download)

## List of Examples

### 1. InEventDeclaration

This example (available [here](./01_InEventDeclaration/)) how to use JavaScript directly within the click event of a button. The code in this example is extremely simple (purposefully): It simply interprets the content (innerText) of an HTML paragraph as a number and increments that by 1. Effectively, this is counting the number of times the button was clicked.

Documentation:

* [JS docs on w3schools](https://www.w3schools.com/js)


### 2. InScriptTag

An event declaration in HTML can hold only very few lines of JavaScript code without becoming hard to read and edit. Thus, it is a much better practice to separate out the JavaScript code from HTML. We can still have it in the same text file but put it into its own area, the "script" tag. 

This [second example](./02_InScriptTag/) does exactly that, providing the exact same functionality as the first example. Additionally, it introduces the concept of functions. 

Documentation:
* [Script Tag](https://www.w3schools.com/Tags/tag_script.asp)  on w3schools. Contains information for the next example as well already.
* [Naming conventions for JS](https://www.w3schools.com/js/js_conventions.asp) for better readability of code. For example, that the curly braces (``{}``) in code should always be opened at the end of the line or that the names of functions and variables should always start with a lowercase character.

### 3. InExternalScriptFile

[This example](./03_InExternalScriptFile) separates the HTML from JS code even further by placing it in a separate file.

Still, the functionality will be the same, simply counting the button clicks.

Documentation:
* [Script Tag](https://www.w3schools.com/Tags/tag_script.asp)  on w3schools.

### 4. JQuery

JQuery can improve JavaScript code a lot. Using this library, the same results can be achieved with less code in a much more declarative style.

The [fourth example](./04_JQuery) counts the clicks again, but with JQuery the HTML elements in this example do not contain any JS any longer, not even the calling of functions needs to be coded in the click event handler any longer, which separates our JS code even further from the HTML, simplifying development of both.

The only thing that needs to be coordinated between the HTML and the JS now is the IDs of the elements - e.g. ``#target`` in JQuery will always get the element with ``id="target"`` in HTML.

Documentation:
* https://www.w3schools.com/jquery/
* https://www.w3schools.com/jquery/jquery_intro.asp
* https://www.w3schools.com/jquery/jquery_syntax.asp

### 5. UseAPI

[This example](./05_UseAPI/) is the first one, in which we need to do something else than just counting clicks.

So far, our code always only worked on information that is contained directly in our HTML document (also known as the DOM - Document Object Model, containing all the HTML elements like the paragraphs, buttons and such). Yet often we will need to access external information as well like data that is stored on a server. Typically, in such cases we will call an API - an Application Programmers Interface, which provides information in a way that programs like our JavaScript code can understand.

One example of such an API is the publically available Dog API that simply lists dog breeds. Our example simply calls that API and counts how many breeds are available currently from that API (our code does not need to do much there, it just uses the ``length`` property of a JS array, the interesting part is the code for calling the API).

Documentation:
* https://dog.ceo/dog-api/documentation/


### For later:

Sometimes we would like to dynamically draw a picture on our website by code (think of maybe drawing a map of your MineCraft world, as just one of many examples). This can be achieved in JS using a [canvas](https://www.w3schools.com/graphics/canvas_drawing.asp).


