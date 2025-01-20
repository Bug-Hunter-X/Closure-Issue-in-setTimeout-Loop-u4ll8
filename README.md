# JavaScript Closure Issue in setTimeout Loop

This example demonstrates a common closure issue in JavaScript when using `setTimeout` within a loop.  The expected behavior is to log numbers 0 through 9 with a one-second delay between each.  However, due to the way closures work in JavaScript, all logs will output 10.

The `bug.js` file contains the problematic code, and `bugSolution.js` demonstrates a solution using an immediately invoked function expression (IIFE) to create a new scope for each iteration of the loop, correctly capturing the value of `i`.