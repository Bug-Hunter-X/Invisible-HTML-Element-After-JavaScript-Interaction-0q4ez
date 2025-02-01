# Invisible HTML Element Bug

This repository demonstrates a common yet easily overlooked bug in HTML and JavaScript.  An HTML element disappears after a JavaScript function modifies its `display` property to `"none"`, but there's no mechanism to restore its visibility. This leads to a situation where the element is permanently hidden without a page refresh.

The `bug.html` file shows the problematic code, while `solution.html` provides a corrected version that addresses this issue.

## Bug Description

A simple button click hides a div element.  However, there is no way to show the div again without manually refreshing the page. The standard solution of setting display to 'block' or other values doesn't work, as the element is still effectively hidden.