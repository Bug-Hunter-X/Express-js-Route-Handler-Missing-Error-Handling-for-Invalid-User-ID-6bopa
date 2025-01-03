# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers:  missing error handling for invalid input.  Specifically, the code lacks proper handling for cases where the user ID is not a valid number.

## Bug

The `bug.js` file contains the buggy code.  It attempts to find a user based on the ID passed in the request parameters. However, it does not handle the scenario where `req.params.id` is not a valid integer, leading to potential errors.

## Solution

The `bugSolution.js` file provides a corrected version of the code.  It includes error handling to check if the user ID is a number and to return an appropriate error response if it is not.