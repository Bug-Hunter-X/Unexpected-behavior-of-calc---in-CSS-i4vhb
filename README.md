# Unexpected behavior of calc() in CSS

This example demonstrates a common issue with the CSS `calc()` function when used with percentages and fixed values, particularly when the parent element's dimensions aren't explicitly defined.  The bug showcases how this can lead to unexpected results, and the solution provides a fix.

## Bug

The `bug.css` file contains the problematic CSS.  The `#container` element tries to subtract 10px from 100% of the parent width, but this fails if the parent doesn't have a defined width.