# Hidden HTML Element Bug

This repository demonstrates a common yet easily overlooked bug in HTML/JavaScript where an element is hidden using JavaScript but never made visible again. The `myFunction` hides the div, but there's no code to show it again leading to a permanently hidden element.

## Bug Description

The `bug.html` file contains a simple HTML structure with a div and a button. Clicking the button hides the div using `style.display = "none";`. The problem lies in the absence of code to reverse this action, making the div permanently invisible after the button is clicked.  This kind of issue can be hard to debug as it only manifests after a user action. 

## Solution

The `solution.html` file corrects this by adding a simple `setTimeout` function that makes the div visible again after a short delay, demonstrating a basic way to resolve the issue.