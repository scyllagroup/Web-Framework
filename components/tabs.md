<div class="breadcrumbs">
[Documentation](/) / Components / Tabs
</div>

# Tabs

## Highlights

*   This component adds no requirements to how you structure your DOM. _Ultimately how you choose to style this component will impact the resulting DOM structure._
*   _Data attributes below should be applied to the element used as a toggle._
*   Use `data-default` to identify the default active tab on load.
*   Use `data-reveal` to provide a CSS query selector to the element that you would like to toggle on/off on click or touch.
*   Tabs can (optionally) be grouped together so only 1 can be active at a time. Create groups with the `data-group` attribute.
*   You can force tab groups to always leave at least 1 tab active with the `data-always-open` attribute.
*   An active tab element will contain the modifier class `.-active` which can be used for styling.
*   By applying a custom `data` attribute above it will imply a truthy condition.

</div>

<div>

## Roadmap

*   Test in IE11, Edge, Chrome, Firefox, [Mac] Safari, [iOS] Mobile Safari.
*   Component works with touch events.
*   Create 1-3 design styles for tabs.
*   Save state and reinitialize from Cookie or LocalStorage
*   Map data attributes to options / properties.
*   Aria testing needs to be performed and appropriate attributes added to markup.

</div>

</div>

</div>

<div class="example -bg-tertiary1">

<div class="flex -pad -wrap-60">

<div>

<div class="tab -active" data-reveal="#hannibal" data-group="1" data-default="" data-always-open="true">Hannibal</div>

<div class="tab" data-reveal=".xfiles" data-group="1">X-Files</div>

<div class="tab" data-reveal=".rickandmorty" data-group="1">Rick and Morty</div>

<div class="tab" data-reveal=".parksandrec" data-group="1">Parks and Recreation</div>

<div class="tab-panel -active" id="hannibal">![](/assets/media/hannibal.jpg)</div>

<div class="tab-panel xfiles">![](/assets/media/xfiles.jpg)</div>

<div class="tab-panel rickandmorty">![](/assets/media/rickandmorty.jpg)</div>

<div class="tab-panel parksandrec">![](/assets/media/parksandrec.jpg)</div>

</div>

</div>

</div>