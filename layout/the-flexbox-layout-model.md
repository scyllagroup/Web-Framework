# The Flexbox Layout Model

The Flexbox Layout Model is our standard, default choice when building row and column based designs. [For browser compatibility information click here.](http://caniuse.com/#feat=flexbox)

## Equal Columns

The default state of our grid framework is to set all columns equal to each other. The following examples all build upon this simple HTML:

<div class="-text-center -styleguide">
<div class="flex">
<div>1</div>
</div>
<div class="flex">
<div>2.1</div>
<div>2.2</div>
</div>
<div class="flex">
<div>3.1</div>
<div>3.2</div>
<div>3.3</div>
</div>
<div class="flex">
<div>4.1</div>
<div>4.2</div>
<div>4.3</div>
<div>4.4</div>
</div>
<div class="flex">
<div>5.1</div>
<div>5.2</div>
<div>5.3</div>
<div>5.4</div>
<div>5.5</div>
</div>
<div class="flex">
<div>6.1</div>
<div>6.2</div>
<div>6.3</div>
<div>6.4</div>
<div>6.5</div>
<div>6.6</div>
</div>
</div>

## Other Sizes

Adjusting the size of our columns is as easy as attaching a modifier class to the container inside. Here are some examples:

<div>
<div class="flex">
<div class="-m-2 -l-2">2/4</div>
<div>1/4</div>
<div>1/4</div>
</div>
<div class="flex">
<div>1/5</div>
<div class="-l-2 -m-2">2/5</div>
<div class="-l-2 t-2">2/5</div>
</div>
<div class="flex">
<div>1/6</div>
<div class="-l-2 -m-2">2/6</div>
<div class="-l-3 -m-3">3/6</div>
</div>
</div>

## Horizontal Alignment

You can justify columns to the start (left), center, or end (right). Their default position is the start.

<div class="row">
<div class="-xs-4">![](/assets/media/justify-content-flex-start.jpg)</div>
<div class="-xs-4">![](/assets/media/justify-content-center.jpg)</div>
<div class="-xs-4">![](/assets/media/justify-content-flex-end.jpg)</div>
</div>
<div>
<div class="flex -fixed">
<div>
These columns are aligned left.
</div>
<div>
These columns are aligned left.
</div>
<div>
These columns are aligned left.
</div>
</div>
<div class="flex -hcenter -fixed">
<div>
These columns are aligned to the center.
</div>
<div>
These columns are aligned to the center.
</div>
<div>
These columns are aligned to the center.
</div>
</div>
<div class="flex -hright -fixed">
<div>
These columns are aligned right.
</div>
<div>
These columns are aligned right.
</div>
<div>
These columns are aligned right.
</div>
</div>
<div class="flex -hbetween -fixed">
<div>
Space is distributed between these columns.
</div>
<div>
Space is distributed between these columns.
</div>
<div>
Space is distributed between these columns.
</div>
</div>
<div class="flex -haround -fixed">
<div>
Space is dsitributed before, between, and after these columns.
</div>
<div>
Space is dsitributed before, between, and after these columns.
</div>
<div>
Space is dsitributed before, between, and after these columns.
</div>
</div>
</div>

## Vertical Alignment

You can align columns to the start (top), center, or end (bottom). By default columns will stretch and be of equal heights.

<div class="row">
<div class="-xs-3">![](/assets/media/align-items-flex-start.jpg)</div>
<div class="-xs-3">![](/assets/media/align-items-center.jpg)</div>
<div class="-xs-3">![](/assets/media/align-items-flex-end.jpg)</div>
<div class="-xs-3">![](/assets/media/align-items-stretch.jpg)</div>
</div>
<div>
<div class="flex -vtop">
<div>
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</div>
<div>
Pellentesque viverra neque diam. Praesent eu lorem ac nibh posuere malesuada. Nam hendrerit eget risus quis interdum. Quisque ut sem vitae sapien semper efficitur. Cras nec magna varius, fermentum dui a, tristique odio. Ut lobortis est ac orci cursus pulvinar. Vestibulum sit amet justo ac massa molestie suscipit.
</div>
<div>
Nullam neque tortor, tempor vitae nulla id, fermentum viverra orci. Pellentesque sodales urna at vulputate convallis. Donec malesuada orci neque, id dictum ex luctus sed. Cras gravida, lacus eu commodo pretium, risus lacus bibendum leo, at imperdiet metus metus eu eros. Etiam dolor metus, accumsan in varius sed, consequat et nulla. Morbi blandit magna vitae erat pharetra, sit amet scelerisque quam vehicula. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Suspendisse sit amet nisi consectetur, faucibus nunc eget, vulputate ex. Proin diam ante, iaculis vitae placerat non, mollis a ligula.
</div>
</div>
<div class="flex -vcenter">
<div>
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</div>
<div>
Pellentesque viverra neque diam. Praesent eu lorem ac nibh posuere malesuada. Nam hendrerit eget risus quis interdum. Quisque ut sem vitae sapien semper efficitur. Cras nec magna varius, fermentum dui a, tristique odio. Ut lobortis est ac orci cursus pulvinar. Vestibulum sit amet justo ac massa molestie suscipit.
</div>
<div>
Nullam neque tortor, tempor vitae nulla id, fermentum viverra orci. Pellentesque sodales urna at vulputate convallis. Donec malesuada orci neque, id dictum ex luctus sed. Cras gravida, lacus eu commodo pretium, risus lacus bibendum leo, at imperdiet metus metus eu eros. Etiam dolor metus, accumsan in varius sed, consequat et nulla. Morbi blandit magna vitae erat pharetra, sit amet scelerisque quam vehicula. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Suspendisse sit amet nisi consectetur, faucibus nunc eget, vulputate ex. Proin diam ante, iaculis vitae placerat non, mollis a ligula.
</div>
</div>
<div class="flex -vbottom">
<div>
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</div>
<div>
Pellentesque viverra neque diam. Praesent eu lorem ac nibh posuere malesuada. Nam hendrerit eget risus quis interdum. Quisque ut sem vitae sapien semper efficitur. Cras nec magna varius, fermentum dui a, tristique odio. Ut lobortis est ac orci cursus pulvinar. Vestibulum sit amet justo ac massa molestie suscipit.
</div>
<div>
Nullam neque tortor, tempor vitae nulla id, fermentum viverra orci. Pellentesque sodales urna at vulputate convallis. Donec malesuada orci neque, id dictum ex luctus sed. Cras gravida, lacus eu commodo pretium, risus lacus bibendum leo, at imperdiet metus metus eu eros. Etiam dolor metus, accumsan in varius sed, consequat et nulla. Morbi blandit magna vitae erat pharetra, sit amet scelerisque quam vehicula. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Suspendisse sit amet nisi consectetur, faucibus nunc eget, vulputate ex. Proin diam ante, iaculis vitae placerat non, mollis a ligula.

</div>
</div>
<div class="flex">
<div>
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
</div>
<div>
Pellentesque viverra neque diam. Praesent eu lorem ac nibh posuere malesuada. Nam hendrerit eget risus quis interdum. Quisque ut sem vitae sapien semper efficitur. Cras nec magna varius, fermentum dui a, tristique odio. Ut lobortis est ac orci cursus pulvinar. Vestibulum sit amet justo ac massa molestie suscipit.
</div>
<div>
Nullam neque tortor, tempor vitae nulla id, fermentum viverra orci. Pellentesque sodales urna at vulputate convallis. Donec malesuada orci neque, id dictum ex luctus sed. Cras gravida, lacus eu commodo pretium, risus lacus bibendum leo, at imperdiet metus metus eu eros. Etiam dolor metus, accumsan in varius sed, consequat et nulla. Morbi blandit magna vitae erat pharetra, sit amet scelerisque quam vehicula. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Suspendisse sit amet nisi consectetur, faucibus nunc eget, vulputate ex. Proin diam ante, iaculis vitae placerat non, mollis a ligula.
</div>
</div>
</div>

## Handling Breakpoints

Sometimes we want to change the size of our columns based on the breakpoint we are in. We can accomplish this by using the modifier classes and the column size combined. We use prefixes for the breakpoints (xs, s, m, l) along with number values (1 - 16) to control the size of the columns. The columns below will highlight to show the active breakpoint. [What are the breakpoints?](breakpoints)

<div>
<div class="flex _highlight-largest-active">
<div class="-xs-12 -s-1 -m-1 -l-1">Extra Small</div>
<div class="-s-3 -m-1 -l-1">Small</div>
<div class="-s-1 -m-3 -l-1">Medium</div>
<div class="-s-1 -m-1 -l-3">Large</div>
</div>
</div>

The following example below takes us through customizing flexbox through major breakpoints:

*   **Medium** or above should show 4 columns of equal width.
*   **Small** should show 1 wide column, and 3 columns of equal width.
*   **Extra Small** has a top row with 2 columns of equal width, the other columns should stack.

<div>
<div class="flex">
<div class="-xs-2 -s-6 -m-3">Col 1</div>
<div class="-xs-2 -s-2 -m-3">Col 2</div>
<div class="-s-2 -m-3">Col 3</div>
<div class="-s-2 -m-3">Col 4</div>
</div>
</div>

## What Flex Does Not Solve

Flex is not always the appropriate class to use. In some instances we want to create a grid of items that are equal width and wrap onto new lines. This is when using the **grid** class is handy. [Learn about the grid class.](WorkingWithGrids)

## Graceful Fallback

Flex is the standard for web layouts moving forward. Clients, however, may request better support for legacy browsers. Currently the fallback for browsers that do not support Flexbox is a stacked layout that mimics a mobile-friendly view.

## Resources

*    W3C - [W3C Candidate Recommendation](https://www.w3.org/TR/css-flexbox-1/)
*    Can I Use - [Browser Compatibility](http://caniuse.com/#feat=flexbox)
