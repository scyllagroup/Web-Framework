<div class="breadcrumbs">
[Documentation](/) / Elements / Colors
</div>

# Colors

A set of modifier classes exist so we can easily apply background and foreground colors to elements that are consistent with brand, UI, or UX guidelines. Including a color pallete in our Web Framework immediately added value for both designers & developers:

*   Our _designers_ are now empowered to define specific colors around client branding, UI styling, and UX feedback.
*   Our _developers_ no longer need to lookup hex or rgb values, they can simply use the appropriate color modifier class.
*   A default color pallete is provided by the Web Framework.
*   Class modifiers exist to apply foreground colors to an element.
    The naming convention is: `-fg-{color-name}`
*   Class modifiers exist to apply background colors to an element.
    The naming convention is: `-bg-{color-name}`

## Define Your Colors

Color names and their values are stored in a SASS `map` named `$colors`. You can find this map in the global config file `./src/_config.scss`. To add a color, just follow the convention already established in the code. You need to provide a name and a value. It's strongly recommended you use an all lower-case name, and no spaces, hyphens, or special characters.

Some things to remember:

*   When you _add_ or _modify_ a color, the Web Framework will generate `.-fg-{color}` and `.-bg-{color}` modifier classes for you.
*   If you _delete_ or _change the name_ of a color, your CSS build might fail. You'll need to search the project for where the old color name was used, and replace it with something else.
*   You may use any of the following types as a color value: named, hex, rgb, rgba, or hsl.

## Reference a Color in SCSS

You'll undoubetedly run across an opportunity to use one of these neatly defined colors from SCSS. This is really easy to do thanks to the `map-get` function provided by SASS. Let's say you are writing a new class and you want to use the `primary1` color:

## Reference a Color in HTML

Since we have modifier classes for each of the colors, we can simply add a class to change the foreground or background color on the fly.

`<div class="-fg-primary1 -bg-secondary1">
  This text would adopt the _primary1_ color.
  But the background would match _secondary1_.
</div>
`

## Brand Colors

<div class="color-boxes">
<div class="-bg-primary1">Primary 1</div>
<div class="-bg-primary2">Primary 2</div>
<div class="-bg-secondary1">Secondary 1</div>
<div class="-bg-secondary2">Secondary 2</div>
<div class="-bg-tertiary1">Tertiary 1</div>
<div class="-bg-tertiary2">Tertiary 2</div>
</div>

## Social Media Colors

<div class="color-boxes">
<div class="-bg-facebook">Facebook</div>
<div class="-bg-flickr">Flickr</div>
<div class="-bg-github">GitHub</div>
<div class="-bg-googleplus">Google Plus</div>
<div class="-bg-instagram">Instagram</div>
<div class="-bg-kickstarter">Kickstarter</div>
<div class="-bg-linkedin">LinkedIn</div>
<div class="-bg-pinterest">Pinterest</div>
<div class="-bg-twitter">Twitter</div>
<div class="-bg-vimeo">Vimeo</div>
<div class="-bg-youtube">YouTube</div>
</div>

## References

*   CSS Color
    [https://developer.mozilla.org/en-US/docs/Web/CSS/color](https://developer.mozilla.org/en-US/docs/Web/CSS/color)