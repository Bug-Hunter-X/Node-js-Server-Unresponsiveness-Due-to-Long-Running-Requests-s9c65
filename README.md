# Node.js Server Unresponsiveness

This repository demonstrates a common issue in Node.js where a server can become unresponsive due to long-running requests blocking the event loop.  The example simulates a request that takes 5 seconds to process, causing other incoming requests to be delayed or ignored.

## Bug Description
The `server.js` file shows a simple HTTP server with a request handler that contains a long-running loop that takes approximately 5 seconds to complete. This blocks the event loop preventing Node.js from handling other requests in a timely manner, causing the server to appear unresponsive.

## Solution
The `serverSolution.js` file demonstrates a solution to this problem using asynchronous operations.

## How to run the examples:
1. Clone the repository.
2. Run `node server.js` to experience the issue.
3. Run `node serverSolution.js` to see the fix in action.