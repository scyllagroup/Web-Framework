<div class="breadcrumbs">
[Documentation](/) / Elements / Tables
</div>

# Tables

## Highlights

*   Default styling is simplistic.
*   Striped rows available.
*   Rows can be highlighted on hover.

## Roadmap

*   Creative team should provide feedback on table styling options that should be made available within the web framework.
*   Be considerate of the frameworks purpose to provide best practices in a bare-bones fashion.

## Table

TBD.

## Striped

TBD.

## Hover Highlight

TBD.

## Responsive Tables

Tables are not naturally resposive, nor is the task of displaying multiple columns of data a trival one for mobile.

Keep in mind that the following CSS solution is only one of many UX improvements we can make to tables. Other solutions require JavaScript code, but offer much more complexity - changing what data it shown, how data is sorted, etc.

Responsive tables can be accomplished by giving the parent container a class `.-scroll-y` which enables the overflow (caused by the table data) to enable a scrollbar.

TBD.

## Scripting Considerations

**Striped rows** use the `nth-of-type` selector to apply a background color appropriately. This works very well, until you begin creating dynamic tables where rows are hidden from view. CSS has yet to provide a combination of selectors to target odd or even rows that are visible as well.

The correct approach to take when hiding rows of data inside of a table is the following:

1.  Choose a row to hide.
2.  Save it's original index position.
3.  Hide the row, but also move the element to the end of the `table`.
4.  When making this row visible again, use it's original index to move it back into place.