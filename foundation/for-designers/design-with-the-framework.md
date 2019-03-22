# The Web Framework for Designers

## The Design Process

<p class="danger">
This page needs work!
<p>

New designers and team members should use htis page to get up to speed with the Web Framework as a design system. Team members can benefit from using this page as a resource and reference when talking about the design process for web based projects.

**Topics:**

1. [Defining Space](#defining-space)
   A step by step guide to creating your first HTML layout and populating it with content.
2. [Styling: Inline vs Stylesheet](#styling-inline-vs-stylesheet)
   Learn when to use inline styles and when it's appropriate to add them to your own stylesheet.
3. [Page Layout Example](#page-layout-example)
   Let's walkthrough how to add a new page layout to any project - following all the best practices and conventions of the Web Framework.
4. [Adobe XD](#adobe-xd)
   With our starter files you can quickly create interactive prototypes using elements, components, and conventions from the Web Framework.

### Defining Space

* Start by carving space from your empty white canvas.
* Use flexbox to create series or rows and columns to create said space.
* Add FPO content and styles to conceptualize the idea you have in mind.
* Think about where you want the spaces to flow transitioning between breakpoints.
* Add any responsive classes or modifiers needed to achieve your goal.
* Discuss CSS positioning - static, relative, absolute, fixed.
* Discuss CSS display or flow - inline, inline-block, block.

### Styling: Inline vs Stylesheet

* Inline styling is great for rapid iteration and exploration of ideas.
* If you wrote it more than once - it probably needs to be a class.
* Global style changes, usually elements, should be made to the framework files.
* Unique components and page layouts should have their own SCSS files in the client files.
* Cleanup in phases - such as finishing a single page layout, or moving from wireframes to prototyping.
* Comment your code so we can review as a team later.
* Follow the Component (C), Element (E), Modifier (M), and Hook (H) convention for CSS use.

### Page Layout Example

* Come up with a semantic name for your page layout.
* Create a new SCSS file, add it so that it compiles with the rest of the project.
* Create the HTML page and attach the new page layout.

### Adobe XD

* Link to download Adobe XD.
* Our starter file for new projects - location, use case.
* Our UI/UX exploration document - location, use case.