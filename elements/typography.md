<div class="breadcrumbs">
[Documentation](/) / Elements / Tables
</div>

# Typography

## Highlights

*   Strip user-agent styling from all standard text elements. Reset to base size and style.
*   Establish specific styles of text (font, size, color, spacing) and create CSS classes to apply.
*   Seperation of concerns between design and SEO.

## Roadmap

*   Continuous research in effective display and use of type.
*   SVG alternative to bullets.

## Text Elements

### Typography Styles

We begin by resetting all font sizes, weights, font families & margins for text elements. Next we construct classes on how we want specific groups of fonts to look and feel. This allows us the freedom to use the heading elements in any way we like, without compromising our choosen formatting. We have the freedom to use the tags for their SEO and semantic benefit and our classes for their styling and presentation.

Classes developed in the base typography are typically things that will be used frequently around the site. Common classes to build are `.header` abd `.sub-header`, which will generally be used to identify page headers and other important titles. It is important that beyound our manual font reset that elements are not further styled with their generic selector tags (i.e. `p` or `h1`). This prevents any cascading issues with referencing the selectors in multiple places, and helps keep our code clean.

We use **rems** as the unit of measure instead of **ems** or **px**. This is because a **rem** value is relative to what we set as the base font size for our `<html>` tag, while **em** is relative to its parent and **px** is static. This ensures that our fonts are consistent across a given project, and that they all adhere to the same scalaing. Our deafult base is 16px. We can change this, for instance, between breakpoints to automatically scale the font size accordingly. Sizes are based on an [augmented 4th scale](http://type-scale.com/?size=16&scale=1.414&text=A%20Visual%20Type%20Scale&webfont=Libre+Baskerville&font-family=%27Libre%20Baskerville%27,%20serif&font-weight=400&font-family-headers=&font-weight-headers=inherit&background-color=white&font-color=%23333).

TBD.

### Lists

Ordered and unordered Lists will follow the same sizing parameters as our basic paragraph text. Bullets appear on the outside, so lines that wrap are nicely aligned to the left.

TBD.

Unordered List (1 rem)

TBD.