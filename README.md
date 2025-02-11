# Express.js Route Handler Missing Error Handling for Invalid User IDs

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input.  Specifically, this example shows a route that fetches a user by ID but fails to handle cases where the ID is not a valid integer.

## Bug

The `bug.js` file contains an Express.js route handler that fetches a user by ID.  However, it lacks error handling for cases where the `userId` parameter is not a valid integer.  This can lead to unexpected behavior or crashes.

## Solution

The `bugSolution.js` file provides a corrected version of the route handler.  It includes error handling to check if the `userId` parameter is a valid integer and returns a 400 Bad Request response if it's not.