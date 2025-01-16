# Unhandled Exception in Node.js HTTP Server

This repository demonstrates an example of an unhandled exception in a Node.js HTTP server and shows how to properly handle it using error handling mechanisms.

## Bug
The `bug.js` file contains a simple HTTP server.  However, if you request the `/error` route, it throws an error without proper handling, causing the server to crash.

## Solution
The `bugSolution.js` file provides a corrected version that uses a `try...catch` block to gracefully handle the error, preventing the server from crashing and allowing for better error reporting.

## How to reproduce
1. Clone this repository.
2. Navigate to the directory.
3. Run `node bug.js`.
4. Open your browser and visit `http://localhost:3000/error` (This will crash the server).
5. Run `node bugSolution.js`
6. Open your browser and visit `http://localhost:3000/error` (This will show an error message instead of crashing.)