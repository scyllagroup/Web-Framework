<div class="breadcrumbs">
[Documentation](/) / Elements / Buttons
</div>

# Buttons

## Highlights

*   Buttons often appear as many different elements such as: `input`, `button`, or `anchor`.
*   Icons can accompany buttons, rectangular or circular.
*   Background and foreground colors can easily be manipulated through the [Colors Pallete](../elements/ColorsPallete).

## Roadmap

*   The structure of the CSS and documentation for buttons is in disarray. I will address this next time we work together with buttons. - Mark
*   Complete the states for buttons:
    `default` or `up`,
    `active` & `focus` & `down`,
    and `disabled`.
*   Creative team should provide feedback on styling options that should be made available within the web framework.
*   Be considerate of the frameworks purpose to provide best practices in a bare-bones fashion.

## Types of Buttons

The three types of buttons are: flat, rectangular, and circular. All buttons are **rectangular** by default.

There are special considerations for **circular**. The child element should be media (gif, png, or svg) and the media should have a 1:1 aspect ratio for the button to remain a perfect circle.

<button class="-flat">Flat</button>
<button>Rectangular</button>

## Flat

## Default

## Circular

Buttons should look similar accross all devices and browsers. So we reset things like the font, background, padding, border, and margins. Also buttons should appear the same regardless of the HTML element they use, like <span class="code"><a></span> or <span class="code"><button></span> or <span class="code"><input></span>.

<button>Button Element</button>

[Anchor Element](#)

Background and foregrounds color classes from the Colors Pallete can be applied.

<button class="-bg-primary1 -fg-white">Primary</button>
<button class="-bg-secondary1 -fg-white">Secondary</button>
<button class="-bg-tertiary1">Tertiary</button>
<button class="-bg-facebook -fg-white">Facebook</button>

Lastly, buttons can be set to stretch to the entire width of their container.

<button class="-block">Stretched</button>