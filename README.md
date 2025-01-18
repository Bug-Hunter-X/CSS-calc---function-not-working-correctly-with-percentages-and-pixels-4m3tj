# CSS calc() Bug

This repository demonstrates a bug in the CSS `calc()` function.  The `calc()` function is not correctly calculating width when percentages and pixels are used together.

## Bug Description

The expectation is that `calc(50% - 10px)` would calculate 50% of the parent container's width and then subtract 10 pixels. However, in some browsers, this calculation is incorrect, resulting in unexpected element widths.

## How to reproduce

1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe the width of the element with the id `myElement`.
4. The width will likely not be 50% of the container's width minus 10px.

## Solution

The provided `bugSolution.css` offers a workaround that ensures consistent and accurate calculations across different browsers. Please refer to `bugSolution.css` for the solution.

## Browser Compatibility

The bug is not consistent across browsers, so testing in various browsers is recommended.