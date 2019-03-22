<div class="breadcrumbs">
[Documentation](/) / Foundation / Breakpoints
</div>

# Breakpoints

## Introduction

Breakpoints, based on the display width of the device, have been established to assist us in building highly adaptable designs and a structure in which we can progressively enhance how we deliver content to the user.

*   Begin your CSS at the mobile breakpoint first.
*   Progressively enhance the display of content as the available space increases.

The following breakpoints have been established but can easily be adjusted in the framework. I'd like to compile some data on common browser sizes for early 2016 and update this so that **Extra Small** targets legacy mobile devices, **Small** targets mobile devices, **Medium** targets tablets and most laptops, and **Large** targets desktop and television environments.

## What are our breakpoints?

| Breakpoint | Measurement | Resolutions | Usage
|:----------:|:-------------------:|------------------------------------------|------:|
| XS | Up To<br>**39.99rem**<br><br>(<= 639px) | 375x667<br>360x640<br>414x736<br>320x568 | 29.84% |
| S | At Least<br>**40rem**<br><br>(>= 640px) | 768x1024 | 5.33% |
| M | At Least<br>**64rem**<br><br>(>= 1024px) | 1366x768<br>1440x900<br>1208x800<br>1600x900 | 22.70% |
| L | At Least<br>**120rem**<br><br>(>= 1920px) | 1920x1080 | 9.58% |

## How do we target specific breakpoints?

Our breakpoints are written in SASS, and will be compiled into media queries when a project is built so that the browsers can interpret them properly. To call a breakpoint in your CSS you would write `@include breakpoint` and then attach a suffix of `-xs`, `-s`, `-m`, or `-l` followed by a CSS declaration.

```
# SCSS file

@include breakpoint-m { 
    /*styles go here */ 
}
```

There are cases where you may want to do something specific for a breakpoint - so a few utlility classes have been made available to perform the following:

*   Target a breakpoint to change the size of a column.
*   Show or hide content based on the breakpoint we are in.
*   Change the behavior of elements in the DOM between breakpoints

With the exception of the **xs-breakpoint**, all breakpoints work from their listed breakpoint and up. Using **breakpoint-m** in your CSS will target all breakpoints from a medium screen and above. The breakpoints cascade in an intuitive manner so that you can use multiple breakpoints on any given element if needed. For instance, if something needs to be 4 columns on the medium breakpoint but needs to be 2 columns on the large breakpoint, the CSS is set up so that it will not overwrite any large breakpoint styles with medium breakpoint styles if both have been defined on your element.

## What are the latest statistics for screen resolutions?

These screen sizes were used to determine our current breakpoint system. It is possible that the values will change as various screen size cycle in and out of use. The goal with the breakpoint system isn't to make a pixel perfect presentation, but to encapsulate a variety of screen sizes within each breakpoint that allow the presentation to continually make sense and stay fluid.

[Stats for the U.S. for March 2019](http://gs.statcounter.com/screen-resolution-stats/all/united-states-of-america/#monthly-201903-201903-bar).

| Resolution | Usage
|:----------:|------:|
| 1920x1080 | 10.02% |
| 375x667 | 8.8% |
| 1366x768 | 8.75% |
| 360x640 | 7.77% |
| 414x736 | 5.38% |
| 768x1024 | 5.26% |
| 1440x900 | 4.44% |
| 375x812 | 3.68% |
| 1536x864 | 3.13% |
| 412x846 | 2.79% |
| 1280x800 | 2.62% |
| 1600x900 | 2.51% |
| 1024x768 | 2.5% |
| 320x568 | 2.36% |
