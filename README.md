# Uncommon HTML Bug: innerHTML and display: none conflict

This repository demonstrates an uncommon bug related to the interaction between `innerHTML` and the `display` style property in HTML.

## Bug Description
The bug arises when attempting to modify the visibility of an element by setting its `style.display` property to `"none"`, after its content has been cleared using `innerHTML`.  This approach does not function as intended.

## Solution
The solution uses a different technique to change element visibility. The recommended approach is to use the `style.display` property before modifying the innerHTML content. If you need to hide an element first, doing so before modifying `innerHTML` is vital.   Alternatively, manipulate the element's CSS classes to control visibility.