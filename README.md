# Uncommon HTML Bug: Incorrect Usage of innerHTML

This repository demonstrates an uncommon bug related to the `innerHTML` property in HTML. Incorrect usage of `innerHTML` when appending content can lead to unexpected results, overwriting existing content instead of appending it properly.

## Bug Description
The primary issue is directly concatenating new HTML content to the existing `innerHTML`. This completely replaces the original content within the element instead of adding the new content at the end.

## Solution
The recommended approach is to create a new element, set its content, and then append it to the existing element using `appendChild()`. This maintains the original content while adding the new content.

## Files
* `bug.html`: Demonstrates the buggy code.
* `bugSolution.html`: Shows the correct way to append content using `appendChild()`.