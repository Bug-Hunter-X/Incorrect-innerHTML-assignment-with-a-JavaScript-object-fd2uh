# Uncommon HTML Bug: Incorrect innerHTML Assignment

This repository demonstrates a subtle bug in HTML where attempting to directly set the `innerHTML` property of an element to a JavaScript object instead of a string results in unexpected behavior.  The `innerHTML` property expects a string; assigning an object will not render its content.  The solution shows the correct way to handle this situation.

## Bug Description
The original code attempts to set the `innerHTML` of a div element to a JavaScript object. This does not render the object's content, leading to an empty div.

## Solution
The solution converts the JavaScript object to a string representation (e.g., using `JSON.stringify`) before assigning it to `innerHTML`, or constructs the HTML string directly.