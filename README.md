# Tailwind CSS @apply Directive Issue with Pseudo-element Selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive doesn't correctly handle classes containing pseudo-element selectors (::before, ::after).

## Bug Description

The `@apply` directive fails to apply styles when a class includes `::before` or `::after` selectors. This leads to unpredictable styling results, potentially affecting other parts of your application.

## Steps to Reproduce

1. Clone this repository.
2. Open `bug.css` to see the buggy implementation.
3. Observe the unexpected behavior in the browser.
4. Compare the result with the corrected implementation in `bugSolution.css`.

## Solution

The bug is solved by using regular CSS rules to style the element instead of relying on `@apply` with pseudo-element selectors. See `bugSolution.css` for a fixed implementation.