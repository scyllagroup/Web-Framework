<div class="breadcrumbs">
[Documentation](/) / Components / Accordions
</div>

# Accordions

## Highlights

*   This component adds no requirements to how you structure your DOM. _Ultimately how you choose to style this component will impact the resulting DOM structure._
*   _Data attributes below should be applied to the element used as a toggle._
*   Use `data-default` to identify the default active accordion on load.
*   Use `data-reveal` to provide a CSS query selector to the element that you would like to toggle on/off on click or touch.
*   Accordions can (optionally) be grouped together so only 1 can be active at a time. Create groups with the `data-group` attribute.
*   You can force accordion groups to always leave at least 1 accordion active with the `data-always-open` attribute.
*   An active accordion element will contain the modifier class `.-active` which can be used for styling.

## Roadmap

*   Test in IE11, Edge, Chrome, Firefox, [Mac] Safari, [iOS] Mobile Safari.
*   Component works with touch events.
*   Create 1-3 design styles for accordions.
*   Prevent accordions from being initialized more than once. We don't want to bind multiple events.
*   Save state and reinitialize from LocalStorage, or Cookie if available.
*   Map data attributes to options / properties for each accordion.
*   ARIA testing needs to be performed and appropriate attributes added to markup. If ARIA attributes are not detected, our script should add them programatically.

TBD.