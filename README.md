# MongoDB $inc Operator Error: Invalid Increment Value

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numerical field by a specified value. However, if you attempt to increment with a non-numerical value, you will encounter an error.

## Bug

The `bug.js` file contains code that attempts to increment a counter field with a string value.  This will result in a MongoDB error.

## Solution

The `bugSolution.js` file provides the correct way to use the `$inc` operator, ensuring the increment value is a number.

## How to reproduce

1. Clone the repository.
2. Ensure you have a MongoDB instance running.
3. Run `bug.js`  You should observe a MongoDB error.
4. Run `bugSolution.js`. This should successfully increment the counter field.