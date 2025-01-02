# CSS Specificity Overrides !important with :hover

This repository demonstrates an uncommon CSS issue where the specificity of a pseudo-class (:hover) overrides an !important declaration.  The unexpected behavior arises because specificity rules in CSS define that :hover has higher precedence than !important.

## Bug Description

The main problem is that while using `!important` is often considered a forceful way to ensure a particular style applies, the specificity of selectors will override it in certain situations.  This example shows that a :hover pseudo-class's inherent specificity can take precedence over the `!important` flag.

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` in a text editor and review the code.
3. Open `bugSolution.css` to view a possible solution.
4. Create an HTML file that includes the CSS and test the behavior of the CSS rules and observe the unexpected behavior.

## Solution

The solution involves re-evaluating the CSS structure and avoiding the use of `!important` in this case.  We can refine the selector specificity or restructure the CSS to correctly render the color as expected.