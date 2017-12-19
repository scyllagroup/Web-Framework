<div class="breadcrumbs">
[Documentation](/) / Components / Carousels
</div>

# Carousels

## Highlights

*   This component adds no requirements to how you structure your DOM. _Ultimately how you choose to style this component will impact the resulting DOM structure._
*   _Data attributes below should be applied to the top level element of your carousel._
*   Use the `data-carousel` attribute to identify the top level element of your carousel.
*   Use the `data-stage` attribute to provide a CSS query selector to the element that you would like to set as the stage element where your carousel slides will be         nested.
*   Use `data-previous` and `data-next` to provide CSS selectors for buttons that will be used for manual transitions.
*   Use the `data-pagination` to provide a CSS selector for the parent element of all pagination elements. Each child element will be assigned a carousel slide in the       order that they appear in the carousel.
*   Use the `data-autoplay` attribute to set whether you'd like the carosel auto transition initially. This takes a `true` or `false` value, and is set to `false` by        default.
*   Each child element of the stage element will be considered a slide. Our slides make use of the `picture` tag to set a specific image a specific breakpoints.
*   A touch event library (ZingTouch) is used to automically apply a swipe event to the stage element. Swiping left or right on mobile devices will transition the           carousel in the direction swiped.
*   Any manual events from a user will stop the carousel from automatically transitioning.



## Roadmap

*   Test in IE11, Edge, Chrome, Firefox, [Mac] Safari, [iOS] Mobile Safari.
*   Create 1-3 design styles for tabs.
*   Save state and reinitialize from Cookie or LocalStorage
*   Map data attributes to options / properties.
*   Aria testing needs to be performed and appropriate attributes added to markup.