# Express.js Route Handler Error
This repository demonstrates a common error in Express.js route handlers:  lack of error handling for invalid input and missing users.
The `bug.js` file contains the erroneous code. The `bugSolution.js` file shows the corrected code with proper error handling.
## Bug
The original code attempts to parse a user ID from the request parameters but fails to handle cases where the ID is not a valid integer or the user is not found.  This can lead to unexpected behavior and crashes. 
## Solution
The solution involves adding explicit checks for invalid input (isNaN) and handling cases where a user is not found by returning a 404 status code.