# Uncommon HTML Bug: Dynamic Script Insertion using innerHTML

This repository demonstrates an uncommon bug in HTML related to dynamically inserting script tags using `innerHTML`.  Directly inserting script tags via `innerHTML` is generally unsafe and can lead to unexpected results and security risks (Cross-Site Scripting - XSS). This example shows the problem and provides a safer alternative.

## Bug Description
The `bug.html` file shows how directly using `innerHTML` to insert a script tag within an HTML element can cause an alert box to unexpectedly appear. This is not a standard practice and should be avoided.

## Solution
The `bugSolution.html` file demonstrates the safer method of dynamically adding a script tag to the DOM. It creates a new script element, sets its `src` or `text` attributes, and then appends it to the document's head.