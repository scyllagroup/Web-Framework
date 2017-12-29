# Guidelines for CSS

## Introduction

Cascading Style Sheets [CSS] started out as a simple way of applying basic design to your HTML. Over time, the CSS Standard has grown more robust - sometimes bluring the lines between User Interface [UI] and User Experience [UX]. Another point of contention is it's nature to broadly define, apply, & inherit styling between HTML elements.

<p class="tip">
**Developers:** Try keeping up to date with the latest recommendations from the W3C. At a bare minimum you should be familiar with all Recommendations [REC], while any Proposed Recommendations [PR] should be on your radar.
<br><br>
[https://www.w3.org/Style/CSS/current-work](https://www.w3.org/Style/CSS/current-work)
</p>

## A quick look at this document

*   We write Sassy CSS [SCSS].
*   The anatomy of CSS: what it means when we say `property`, `value`, `block`, `rule`, and `ruleset`.
*   Establish naming & usage conventions for `ID` selectors & `Class` selectors.
*   Discover how our Web Framework builds our stylesheets.
*   Other best practices and rules for working on CSS in large teams.
*   References for further reading and understanding.

## Writing CSS

### Anatomy of CSS

This is the basic structure of writting CSS code:

`p {color: blue;}`

Where the `p` references all paragraph tags `<p>` in the given css scope, and is referred to as a selector. What follows the selector is an object that contains rules or **styles** that will be applied to the selector preceeding the rule set, known as the **declaration**. Every style follows the same written convention; define the property you want to change, define the new property value, and then end the line with a semicolon. Every declaration begins and ends with a set of `{ }` to keep them contained and scoped to the selector(s) that preceeded them.

### What is SCSS

Or better know as SASS, SCSS is a simply an extension of CSS that allows us to better manage and maintain our ever-growing library of styles. It affords us the opportunity to manage large sets of styles by breaking them into more manageable files, and reduce complexity by making it easier to understand the inheritance going on within our definitions. SASS and compilation allows us to define and use variables and blocks of styles (mixins) in our code as well. [Learn more about SASS here.](http://sass-lang.com/)

SCSS isn't something that the browser understands natively, so we have to transpile it. Part of the build system included with the Web Framework is dedicated to finding all the relevant, in-use SCSS files and concatenate, transpile, and minify the output into a CSS file.

### Naming & Usage Conventions for IDs & Classes

*   When should an ID be used and when should a class be used?
*   What are some different use cases for the class attribute?

| Format | Type | Explanation | Usage |
|--------|------|-------------|-------|
| **#id** | Component | Represents a major or unique page component, non-repeatable. | Infrequent |
| **.class** | Element | Represents repeatable components or elements. | Frequent |
| **.-class** | Modifier | Used to modify, change, or update properties of specific elements or components. They do not exist on their own. | Frequent |
| **._class** | Hook | Should only be used as a way to target elements from JavaScript code. | Rare |

### SCSS & The Build System

TBD.

## Best Practices

In general it's best to keep all CSS written in a correctly scoped stylesheet. Within the framework project every CSS file is labeled appropriately and put into an appropriate folder. For example, the CSS for **buttons** is located in the **elements** folder and titled **buttons.scss**. This keeps all our CSS rulesets grouped neatly, and makes them easier to find and edit. 

One thing to avoid, unless absolutely necessary, is writing inline CSS rules. Because inline styles are very specific styles within CSS rules, they'll overwrite almost every other style applied to that element. This can lead to confusion among the development team and even impede development. Most of the time your CSS should be able to be written within a file, commented, and should be easy for anyone else working with the project to locate.

When writing styles using the framework, its important to keep in mind that we don't try to create adaptive presentations. Our code is not written to look perfect on every available screen size, but to think mobile first and build up from there.

## References

*   CSS Syntax - [https://developer.mozilla.org/en-US/docs/Web/CSS/Syntax](https://developer.mozilla.org/en-US/docs/Web/CSS/Syntax)
*   CSS Selectors - [https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)