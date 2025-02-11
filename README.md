# JavaScript - Handling Null and Undefined

This repository demonstrates a common error in JavaScript and its solution. The `bug.js` file contains a function that attempts to access the length property of an argument that may be null or undefined. This causes a `TypeError`. The `bugSolution.js` file provides a solution to this problem.

## Problem
The problem lies in the function `foo()`. If the function is called with an undefined value, it will throw a `TypeError` because `undefined` does not have a `length` property.  This occurs because the code doesn't explicitly check for `undefined`. 

## Solution
The solution involves adding an explicit check for `undefined` before attempting to access the `length` property.  The updated function now correctly handles `null` and `undefined` inputs, returning 0 in both cases. 