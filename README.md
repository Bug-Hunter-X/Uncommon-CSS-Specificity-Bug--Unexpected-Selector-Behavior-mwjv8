# Uncommon CSS Specificity Bug

This repository demonstrates an uncommon bug related to CSS specificity. The bug arises when combining class and ID selectors in a way that leads to unexpected behavior regarding which styles are applied.

## Bug Description

The unexpected behavior involves the order in which CSS selectors are applied.  Many developers might intuitively assume that an ID selector (`#id`) will always override a class selector (`.class`), but this isn't always the case when dealing with complex selector combinations.

## How to Reproduce

1. Clone this repository.
2. Open `bug.css` to see the CSS code with the problematic selectors.
3. Open `index.html` and inspect the element with the relevant classes and ID to see the unexpected width. (If index.html is not provided, create an html file to test the CSS rule)

## Solution

The solution involves a careful understanding of CSS specificity and how selectors are matched against elements. The solution involves using more appropriate selectors to resolve the specificity conflicts, thus ensuring the intended style is applied. See `bugSolution.css` for a corrected approach.

## Lessons Learned

This example highlights the importance of understanding CSS specificity rules.  Even seemingly straightforward selector combinations can produce surprising results if the intricacies of specificity aren't fully grasped.  Always test your CSS thoroughly to prevent unexpected behavior.