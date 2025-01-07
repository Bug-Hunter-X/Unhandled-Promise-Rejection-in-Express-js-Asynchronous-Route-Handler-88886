# Unhandled Promise Rejection in Express.js Async Route Handler

This repository demonstrates a common error in Express.js applications: improper handling of asynchronous operations within route handlers.  The `bug.js` file showcases a route that uses a `Promise` but lacks robust error handling.  The result is that if the asynchronous operation fails, the error is only logged to the console and no appropriate response is sent back to the client.

The `bugSolution.js` file provides a corrected version, demonstrating best practices for handling errors in asynchronous Express.js routes.  The solution employs a `try...catch` block to catch and handle potential errors and sends an appropriate error response to the client. 

This example highlights the importance of comprehensive error handling in asynchronous server-side code to ensure application stability and provide meaningful feedback to users.