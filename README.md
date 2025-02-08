# MongoDB $inc Operator Error
This repository demonstrates a common error when using the `$inc` operator in MongoDB. The `$inc` operator is designed to increment a numerical field by a specified value. Attempting to use it with a string value will result in an error. 

## Bug Description
The bug arises from using a string value ("1") instead of a numeric value (1) with the `$inc` operator.  MongoDB expects a number to increment a field and throws an error if given a string.

## Solution
The solution is to ensure you pass a numeric value to the `$inc` operator to increment the field correctly.

## How to reproduce the error
1. Run the code in `bug.js`.
2. Observe the error message in the console.

## How to fix the error
1. Run the code in `bugSolution.js`.