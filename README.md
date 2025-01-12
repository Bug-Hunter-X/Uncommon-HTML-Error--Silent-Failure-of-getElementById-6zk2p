# Uncommon HTML Error: Silent Failure of getElementById

This repository demonstrates an uncommon error in HTML that can be tricky to debug. The error involves attempting to access a non-existent element using `document.getElementById()`.

## The Bug
The `bug.html` file contains a script that tries to get an element with the ID "nonExistentElement."  Since this element does not exist in the HTML, the script's `if` condition is never met and the code inside doesn't execute. Importantly, there's no error message or warning in the browser's console, making the error difficult to find.

## The Solution
The `bugSolution.html` file corrects the issue by properly checking if the element exists before attempting to manipulate it and includes robust error handling by using a try-catch block.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe that there's no error message, but the expected change to the non-existent element doesn't happen.
4. Open `bugSolution.html` to see the corrected code.