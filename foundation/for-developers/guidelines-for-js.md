# Guidelines for JavaScript

## Introduction

The purpose of this page is to define a set of standards and best practices when working with JavaScript. The overarching themes of the next few sections are:

*   Establish best practices that we are all cognizant of during implementation phases.
*   JavaScript components and widgets will be coded as classes in ES6, transpiled down by a Gulp task.
*   Inline JavaScript should make use of IIFYs and should rarely be used outside of initializing a widget or component.

## Writing JavaScript

*    We write our code using the latest ECMAScript standard - taking full advantage of the language even if the browsers do not support some of the features.
*    Whether you are writing a component or a utility, we write them as `classes` so our library is modular, and our final output can be lean.
*    Our build system, detailed later, utilizes `babel` to transpile our code to something actually supported by our target browsers and devices.

### Latest ECMAScript features

TBD.

### Features That Need to be Transpiled

<!--*     List the features that need to be transpiled due to our target device & browsers.-->
*   Spread Operators
*   Arrow Functions

TBD.

## Build System

TBD.

### Role of WebPack

TBD.

### Role of Babel

TBD.

### Role of ESLINT

TBD.

### Useful Command Line Arguments

TBD.

## App.js

TBD.

### Architecture

Blocks of JS code may intentionally require different execution times. Sometimes we will write a script that we desire _immediate execution_ and other times we may wish for the _page to finish loading_ . Other times, we may execute immediately and allow our code itself to determine the next steps. So our architecture needs to support this type of lazy loading - where scripts can be executed when we desire, no matter their place in the HTML.

I've used [the Revealing Module Pattern](https://addyosmani.com/resources/essentialjsdesignpatterns/book/#revealingmodulepatternjavascript) to initiate the main object, _app_, in the global namespace and return some public methods which can be called by the widgets we create.

### The App Variable

[View the source of "app.js".](~/assets/js/app.js)

Our initial architecture, the app variable, does not use this pattern. We assign it to a variable in the global namespace so we can write an API & access its methods publicly. This is a work in progress. The API has the following methods available:

### Components

TBD.

<table>
<thead>
<tr>
<th>Method</th>
<th>Parameters</th>
<th>More Information</th>
</tr>
</thead>
<tbody>
<tr>
<td>**Queue**</td>
<td><small>**Delay**
Delay defines when the script will execute.
0: Execute immediately (default)
1: Execute on page ready
2: Execute on window load

**Order**
An integer that will eventually be used for prioritizing the order in which scripts are ran.

**Script**
The anonymous function to be executed.

**Variable Name**
* Not implemented yet. Optionally assign the function to a name in the global namespace for public access.</small></td>
<td>Use queue to initialize your own widgets.</td>
</tr>
<tr>
<td>**Performance**</td>
<td></td>
<td>Helps measure performance of blocks of code. Outputs performance data to the console.</td>
</tr>
<tr>
<td>**Storage**</td>
<td></td>
<td>Assists with usage of Cookies & Local Storage.</td>
</tr>
<tr>
<td>**Preloader**</td>
<td><small>**Target Element**
A jQuery selector for the element to disable.

**Disable Form Elements and Links**
A boolean value that determines if we disable form elements and anchor links on the page until the Ajax query is complete.
true: disables elements until complete (default)
false: does not disable any elements</small></td>
<td>Assists with our Ajax calls allowing us to generically apply a preloader graphic and disable all form elements and links inside of a DOM element until the Ajax call is complete. * Not implemented</td>
</tr>
</tbody>
</table>

### Utilities

TBD.

## Resources

TBD.

### Commonly Used 3rd Party Libraries

The following JS libraries are used (some optionally):

*   VueJS - [Website](https://vuejs.org/)
*   Modernizr - [Website](https://modernizr.com), [Our Custom Build](https://modernizr.com/download?canvas-cssanimations-customevent-eventlistener-flexbox-flexboxlegacy-flexboxtweener-geolocation-history-json-localstorage-regions-svg-touchevents-video-websockets-setclasses)
*   GSAP - [Website](http://greensock.com/gsap)
*   ZingTouch - [Website](https://zingchart.github.io/zingtouch/)