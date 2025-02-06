# CSS :hover Pseudo-class Issue on Nested Elements

This repository demonstrates a peculiar issue with the CSS `:hover` pseudo-class when applied to nested elements.  The expected behavior is that the inner `<div>` changes color when hovering over the outer `<div>`. However, under certain circumstances, this does not occur.

## Bug Report

The provided `bug.css` file contains CSS code exhibiting this unexpected behavior.  The `bug.html` (or similar) file shows the HTML structure. The problem is that the inner `<div>` with class `inner-div` doesn't change its background color when hovering over the outer `<div>` with class `outer-div`.

## Solution

The solution, found in `solution.css`, addresses this issue by ensuring that proper specificity is maintained to correctly target the nested element.   This is often related to a cascade or specificity issue where other styles override the hover effect.  Additional explanations can be found in the comments within `solution.css`.