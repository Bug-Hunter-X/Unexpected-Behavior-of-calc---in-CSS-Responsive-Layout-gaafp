# Unexpected Behavior of calc() in CSS Responsive Layout

This repository demonstrates a subtle bug involving the `calc()` function in CSS when used for responsive layouts. The issue arises from inconsistencies in how different browsers interpret and render the `calc()` expression, particularly when subtracting pixel values from percentages.

## Bug Description

The `calc()` function is intended to allow dynamic calculations within CSS property values.  However, older browsers or those with limited CSS support may not handle `calc()` expressions reliably, especially those involving mixed percentage and pixel units.  This can lead to unexpected layout behavior.

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` to see the problematic CSS.
3. Create a simple HTML file (e.g., `index.html`) containing a `div` element.
4. Link the `bug.css` file to your HTML.
5. Observe the width of the `div` in different browsers. You may notice discrepancies compared to the expected width.

## Solution

The solution involves using a more reliable and widely compatible approach to achieve the same responsive layout behavior.  See `bugSolution.css` for the improved CSS code.