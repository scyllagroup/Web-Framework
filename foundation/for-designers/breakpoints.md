<div class="breadcrumbs">
[Documentation](/) / Foundation / Breakpoints
</div>

# Breakpoints

## Introduction

Breakpoints, based on the display width of the device, have been established to assist us in building highly adaptable designs and a structure in which we can progressively enhance how we deliver content to the user.

*   Begin your CSS at the mobile breakpoint first.
*   Progressively enhance the display of content, including additions to feature or function.

The following breakpoints have been established but can easily be adjusted in the framework. I'd like to compile some data on common browser sizes for early 2016 and update this so that **Extra Small** targets legacy mobile devices, **Small** targets mobile devices, **Medium** targets tablets and most laptops, and **Large** targets desktop and television environments.

## What are our breakpoints?

| Breakpoint | Measurement | Resolutions | Usage
|:----------:|:-------------------:|------------------------------------------|------:|
| XS | Up To<br>**40rem**<br><br>(639px-) | 375x667<br>360x640<br>414x736<br>320x568 | 29.84% |
| S | At Least<br>**40rem**<br><br>(640px+) | 768x1024 | 5.33% |
| M | At Least<br>**64rem**<br><br>(1024px+) | 1366x768<br>1440x900<br>1208x800<br>1600x900 | 22.70% |
| L | At Least<br>**120rem**<br><br>(1920px+) | 1920x1080 | 9.58% |

## How do we target specific breakpoints?

There are cases where you may want to do something specific for a breakpoint - so a few utlility classes have been made available to perform the following:

*   Target a breakpoint to change the size of a column.
*   Show or hide content based on the breakpoint we are in.
*   Change the behavior of elements in the DOM between breakpoints

TBD.

## What are the latest statistics for screen resolutions?

[Stats for the U.S. for October 2017](http://gs.statcounter.com/screen-resolution-stats/all/united-states-of-america/#monthly-201710-201710-bar).

| Resolution | Usage
|:----------:|------:|
| 375x667 | 10.46% |
| 360x640 | 10.21% |
| 1366x768 | 10.09% |
| 1920x1080 | 9.58% |
| 1440x900 | 5.50% |
| 768x1024 | 5.33% |
| 414x736 | 5.21% |
| 320x568 | 3.96% |
| 1280x800 | 3.82% |
| 1600x900 | 3.29% |