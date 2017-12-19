<div class="breadcrumbs">
[Documentation](/) / Components / Modals
</div>

# Modals

## Highlights

*   This component adds no requirements to how you structure your DOM. _Ultimately how you choose to style this component will impact the resulting DOM structure._
*   The overlay accompanying modals comes in two themes: (1) a dark background [by default], (2) and a light background if you use the `-light` modifier class.
*   Use the `data-modal` attribute on a `button`, `link`, or other clickable element to pass a CSS selector for the top level element of the modal. 

## Roadmap

*   Test in IE11, Edge, Chrome, Firefox, [Mac] Safari, [iOS] Mobile Safari.
*   Component works with touch events.
*   Address dynamic content, such as an XMLHttpRequest, and integrate wsome visual feedback to the user. A utility class for a loader should be added to the Web Framework.
*   Scrolling should be completely disabled outside of the currently open modal. We can trap that event and stop it from propagating. We can probably avoid DOM manipulation.
*   Modals can be dynamic height, width, or set to full height, full width, or full screen.
*   ARIA testing needs to be performed and appropriate attributes added to markup. If ARIA attributes are not detected, our script should add them programatically.
<!--
TBD.

# Modal Content

Any content can be placed here, including full HTML that makes use of grids, or full-screen multimedia, etc.

TBD.

# Modal Content

Any content can be placed here, including full HTML that makes use of grids, or full-screen multimedia, etc.
-->