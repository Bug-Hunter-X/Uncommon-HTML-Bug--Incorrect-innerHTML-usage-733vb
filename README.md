# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates a subtle bug in HTML that can be difficult to track down. The bug involves attempting to modify the `innerHTML` property of an element that does not exist in the DOM.  This action will not throw an error and may lead to unexpected behavior.

## Bug Description
The `bug.html` file contains Javascript code that attempts to modify the `innerHTML` property of a non-existent element.  The `bugSolution.html` file demonstrates the correct way to handle this situation by first checking for the existence of the element using `getElementById()`.

## How to reproduce the bug
1. Open `bug.html` in your browser.
2. Observe that the text "This text won't show" does not appear, while "This text will show" appears correctly.

## Solution
The `bugSolution.html` file demonstrates the solution. It checks if the element exists before attempting to modify its `innerHTML`. This is a simple but crucial step for preventing unexpected behavior.