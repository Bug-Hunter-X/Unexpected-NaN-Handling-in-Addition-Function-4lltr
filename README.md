# Unexpected NaN Handling in JavaScript Addition Function

This repository demonstrates a subtle bug in a JavaScript function designed to add two numbers. The function handles null values correctly, returning 0 if either input is null. However, it fails to handle NaN (Not a Number) values appropriately. This behavior can be unexpected and lead to errors in applications.

The `bug.js` file contains the buggy code, and `bugSolution.js` provides a corrected version that explicitly handles NaN values.

## Bug
The original function returns NaN if either input is NaN, which might not be the desired behavior in all cases. 

## Solution
The solution explicitly checks for NaN values using `isNaN()` and handles them appropriately, returning 0 or throwing an error, depending on the preferred behavior. 